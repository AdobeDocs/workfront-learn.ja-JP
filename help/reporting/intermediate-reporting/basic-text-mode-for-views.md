---
title: ビューの基本的なテキストモードを理解する
description: テキストモードとは何か、キャメルケースとは何か、およびWorkfrontのビューで使用できる基本的な「プラグアンドプレイ」テキストモードについて説明します。
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 11367
exl-id: 156e5510-4a51-449f-9c8c-e16fdd8ea23d
source-git-commit: 818ee105af32589cb0e297e6f419a4a449a60052
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# ビューの基本的なテキストモードを理解する


>[!IMPORTANT]
>
>前提条件：
>
>* レポート要素について
>* レポートコンポーネントについて
>* 基本ビューの作成


>[!TIP]
>
>* テキストモードをより深く理解するために、録画されたウェビナーイベントを見ることをお勧めします [エキスパートへの質問 — テキストモードレポートの概要](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=en)（長さ 1 時間）。
>* テキストモードの詳細については、 [高度なレポート](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=en) チュートリアルは全部で 5 時間半です。


このビデオでは、次のことを学習します。

* テキストモード
* ラクダの例とは
* ビューで使用できる基本的な「プラグアンドプレイ」テキストモード

>[!VIDEO](https://video.tv.adobe.com/v/3410571/?quality=12)

## タスク — 4 親ビュー

最初にタスク名と親名の列を作成し、次のテキストモードを使用して他の 3 つの列を作成します。

### タスク — 親名の親

```
displayname=Parent of Parent Name
linkedname=parent
namekey=view.relatedcolumn
namekeyargkey.0=parent
namekeyargkey.1=name
querysort=parent:parent:name
textmode=true
valuefield=parent:parent:name
valueformat=HTML
```

### タスク — 親名の親の親

```
displayname=Parent of Parent of Parent Name
linkedname=parent
namekey=view.relatedcolumn
namekeyargkey.0=parent
namekeyargkey.1=name
querysort=parent:parent:parent:name
textmode=true
valuefield=parent:parent:parent:name
valueformat=HTML
```

### タスク — 親名の親の親

```
displayname=Parent of Parent of Parent of Parent Name
linkedname=parent
namekey=view.relatedcolumn
namekeyargkey.0=parent
namekeyargkey.1=name
querysort=parent:parent:parent:parent:name
textmode=true
valuefield=parent:parent:parent:parent:name
valueformat=HTML
```

![4 つの親ビューを示す画面画像](assets/4-parents-view.png)

## ユーザー — ユーザービューでリストを表示する反復

### ユーザー — すべてのジョブの役割

```
displayname=All job roles
listdelimiter=<p>
listmethod=nested(userRoles).lists
textmode=true
type=iterate
valuefield=role:name
valueformat=HTML
```

### ユーザー — プライマリを示すすべてのジョブロール

```
displayname=All Job Roles showing primary
listdelimiter=<p> 
listmethod=nested(userRoles).lists 
textmode=true
type=iterate 
valueexpression=IF({user}.{roleID}={role}.{ID},CONCAT("** ",{role}.{name}," **"),{role}.{name})
valueformat=HTML
```

### ユーザー — すべてのチーム

```
displayname=All teams
listdelimiter=<p>
listmethod=nested(teams).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

>[!NOTE]
>
>UI からアクセスできるチームフィールドがあり、すべてのチームをコンマで区切って表示しますが、上のテキストモードを使用すると、各チームが別々の行に表示されます。


### User - All groups

```
displayname=All groups
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valuefield=group:name
valueformat=HTML
```

### User — ホームグループを表示するすべてのグループ

```
displayname=All groups showing home group
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valueexpression=IF({user}.{homeGroupID}={group}.{ID},CONCAT("** ",{group}.{name}," **"),{group}.{name})
valueformat=HTML
```


### ユーザー — ダイレクトレポート

```
displayname=Direct reports
listdelimiter=<p>
listmethod=nested(directReports).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

### ユーザー — 将来の PTO

```
displayname=Future PTO
listdelimiter=<br>
listmethod=nested(reservedTimes).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=IF({startDate}>$$TODAY,CONCAT({startDate}," - ",{endDate}),"")
valueformat=HTML
width=150
```

![ユーザーリスト表示を示す画面画像](assets/user-lists-view-large.png)

## タスク — タスクの割り当てを表示し、ステータスを操作する方法

```
displayname=Assignments and Status
listdelimiter=<br>
listmethod=nested(assignments).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=CONCAT({assignedTo}.{name},IF(ISBLANK({assignedTo}.{name}),"",IF({status}="AA"," - Requested",IF({status}="AD"," - Working"," - Done"))))
valueformat=HTML
width=150
```

![割り当てビューとステータスビューを示す画面画像](assets/assignments-and-status-view.png)


## タスク — 複数のタスクの割り当てに関する役割と割り当てを表示する方法

### タスク — 役割+時間

```
displayname=Role+hours
listdelimiter=<li>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT({role}.{name}," (",round({workRequired}/60,2),")")
valueformat=HTML
```

### タスク — 割り当て+割り当て率

```
displayname=Assignment+percent
valueexpression=CONCAT({assignedTo}.{name}," (",{assignmentPercent},")")
listdelimiter=<li>
listmethod=nested(assignments).lists
valueformat=HTML
textmode=true
type=iterate
```

![割り当てビューと役割ビューを示す画面画像](assets/assignments-roles-and-percent-view.png)

## タスク — プロジェクト間の先行タスクと後続タスク

### タスクフィルター（オプション）

**1 つ以上のクロスプロジェクトの先行タスクを持つすべてのタスクを表示する**

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

### タスク — 前任者名とプロジェクトの前任者が次の場所にあることを表示

```
displayname=Predecessor names
listdelimiter=<br>
listmethod=nested(predecessors).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=CONCAT("TASK = ",{predecessor}.{name}," >> PROJECT = ",{predecessor}.{project}.{name})
valueformat=HTML
width=150
```

### タスク — 後続の名前を表示し、プロジェクトの後続が

```
displayname=Successor names
listdelimiter=<br>
listmethod=nested(successors).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=CONCAT("TASK = ",{successor}.{name}," >> PROJECT = ",{successor}.{project}.{name})
valueformat=HTML
width=150
```

### タスク — 先行タスクの予定完了日を表示します

```
displayname=Predecessor projected completion dates
valueformat=atDate
listdelimiter=
textmode=true
width=90
stretch=0
valuefield=predecessor:projectedCompletionDate
type=iterate
listmethod=nested(predecessors).lists
shortview=false
```

### タスク — 先行タスクの進捗状況ステータスを表示します

```
displayname=Predecessor progress status
listdelimiter=<br>
listmethod=nested(predecessors).lists
shortview=false
stretch=0
textmode=true
type=iterate
valueexpression=IF({predecessor}.{progressStatus}="OT","On Time",IF({predecessor}.{progressStatus}="LT","Late",IF({predecessor}.{progressStatus}="BH","Behind","At Risk")))
valueformat=HTML
width=90
```

### タスク — プロジェクト間の先行プロジェクトのプロジェクトの完了率を表示します

```
displayname=Predecessor project percent complete
listdelimiter=<br>
listmethod=nested(predecessors).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=IF({isCP}=true,CONCAT({predecessor}.{project}.{percentComplete},"%"),"")
valueformat=HTML
width=150
```

![プロジェクト間の先行タスクおよび後続タスクビューを示す画面画像](assets/cross-project-predecessors-and-successors.png)


## タスク — 割り当て済みの担当者と各担当者を割り当てた担当者をすべて示す反復

```
displayname=All assignees and requesters
listdelimiter=<p>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT("Assigned To: ",{assignedTo}.{name},"; Requested By: ",{assignedBy}.{name})
valueformat=HTML
```

![割り当て済みの担当者と各担当者を割り当てた担当者をすべて示す画面画像](assets/all-assignees-and-requesters.png)

## タスク/プロジェクト — プロジェクトまたはタスク上のすべてのカスタムフォームを表示する反復

```
displayname=All Forms Assigned
listdelimiter=<p>
listmethod=nested(objectCategories).lists
textmode=true
type=iterate
valuefield=category:name
valueformat=HTML
```

![プロジェクト上のすべてのカスタムフォームを示す画面画像](assets/all-custom-forms-on-a-project.png)


## プロジェクト — イテレーションで、プロジェクトビューの解決可能なすべての主要連絡先が表示されます

```
displayname=Requestor
listdelimiter=<br>
listmethod=nested(resolvables).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=owner:name
valueformat=HTML
width=150
```

![解決可能なプライマリ連絡先を示す画面画像](assets/primary-contacts-for-resolvables.png)

## プロジェクト — すべてのプロジェクトチームメンバーを示す反復

```
displayname=Project Team Members
listdelimiter=<br>
listmethod=nested(projectUsers).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=user:name
valueformat=HTML
```

![すべてのプロジェクトチームメンバーを示す画面画像](assets/all-project-team-members.png)

## プロジェクト — プロジェクトの解決可能なすべての問題の entryDate を示す反復

```
displayname=Resolvables entry date
linkedname=direct
listdelimiter=<br>
listmethod=nested(project.resolvables).lists
listsort=string(description)
querysort=description
section=0
textmode=true
type=iterate
valuefield=entryDate
valueformat=HTML
```

![プロジェクトで解決可能なすべての問題の entryDate を示す画面画像](assets/resolvables-entry-date.png)

## プロジェクト — 元のプロジェクト要求者のホームグループを表示します

```
displayname=Requestor home group
linkedname=direct
namekey=name
querysort=convertedOpTaskOriginator:homeGroup:name
textmode=true
valuefield=convertedOpTaskOriginator:homeGroup:name
valueformat=HTML
```

![プロジェクト要求者のホームグループを示す画面イメージ](assets/requestor-home-group.png)

## プロジェクト — プロジェクトがリクエストキューかどうかを表示します

```
querysort=queueDef:isPublic
valueformat=val
description=0 (None), 1 (Public), 2 (Private), 3 (Company), 4 (Group)
linkedname=direct
textmode=true
enumtype=PROJ
valuefield=queueDef:isPublic
namekey=status
type=enum
enumclass=com.attask.common.constants.ProjectStatusEnum
displayname=Public Selection
```

![プロジェクトが要求キューかどうかを示す画面画像](assets/project-is-a-request-queue.png)

## 問題 — すべての解決プロジェクトチームメンバーを示す反復

```
displayname=Resolve Project: Team Members
listdelimiter=<br>
listmethod=nested(resolveProject.projectUsers).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=user:name
valueformat=HTML
width=150
```

![すべての解決プロジェクトチームメンバーを示す画面画像](assets/all-resolve-project-team-members.png)

## 問題 — イシューの主要連絡先のすべてのチームを示す反復

```
displayname=Requestor Teams
listdelimiter=<br>
listmethod=nested(owner.teams).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=name
valueformat=HTML
width=150
```

![すべての主要連絡先チームを示す画面画像](assets/all-primary-contact-teams.png)

## ドキュメント — ドキュメントレポート内のフォルダを示す反復

```
displayname=Folder
listdelimiter=<br><br>
listmethod=nested(folders).lists
textmode=true
type=iterate
valuefield=name
valueformat=HTML
```

![ドキュメントレポート内のフォルダを示す画面画像](assets/folder-in-a-document-report.png)

## ドキュメント — ドキュメントレポート内の親フォルダーを示す反復処理

```
displayname=Parent Folder
listdelimiter=<br><br>
listmethod=nested(folders).lists
textmode=true
type=iterate
valuefield=parent:name
valueformat=HTML
```

![ドキュメントレポート内の親フォルダーを示す画面画像](assets/parent-folder-in-a-document-report.png)

## ドキュメント — ドキュメントの承認日

```
displayname=Document Approval Dates
valueformat=HTML
listdelimiter=<br>
linkedname=direct
textmode=true
listsort=string(description)
valuefield=approvalDate
type=iterate
listmethod=nested(approvals).lists
shortview=false
section=0
```

![ドキュメント承認日ビューを示す画面画像](assets/document-approval-dates.png)

## プルーフの承認

### 配達確認の承認 — プロジェクト名を表示

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name 
valueformat=HTML
```

### 配達確認の承認 — タスク名を表示

```
displayname=Task Name
textmode=true 
valuefield=documentVersion:document:task:name 
valueformat=HTML
```

![配達確認の承認のプロジェクトとタスクを示す画面画像](assets/proof-approval-project-and-task.png)
