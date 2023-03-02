---
title: フィルターの基本的なテキストモードについて
description: テキストモードとは何か、キャメルケースとは何か、およびWorkfrontのレポートフィルターで使用できる基本的な「プラグアンドプレイ」テキストモードについて説明します。
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# フィルターの基本的なテキストモードについて

>[!IMPORTANT]
>
>前提条件：
>
>* レポート要素について
>* レポートコンポーネントについて
>* 基本フィルターの作成


>[!TIP]
>
>* テキストモードをより深く理解するために、録画されたウェビナーイベントを見ることをお勧めします [エキスパートへの質問 — テキストモードレポートの概要](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=en)（長さ 1 時間）。
>* テキストモードの詳細については、 [高度なレポート](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=en) チュートリアルは全部で 5 時間半です。



このビデオでは、次のことを学習します。

* テキストモード
* ラクダの例とは
* レポートフィルターで使用できる基本的な「プラグアンドプレイ」テキストモード

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12)


## タスク — 「自分の部分で完了」とマークしたタスクを除外します

次のテキストモードでは、ユーザーが「Done with My Part」とマークしたタスクが除外されます。 必要な操作は、タスクフィルターを作成し、必要なフィルタールールを追加してから、テキストモードに切り替えて、フィルターに表示される任意のテキストモードの後に下のコードを貼り付けるだけです。

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

## タスク — 承認待ちのすべてのタスクを表示する

```
approvalProcessID_Mod=notblank
currentUserApproversMM:ID=$$USER.ID
currentUserApproversMM:ID_Mod=in
currentUserApproversMM_Join=allowingnull
```

## タスク — 自分が承認したすべてのタスクを表示する

任意のフィルターでタスクレポートを作成し、「フィルター」タブに移動して、「テキストモードに切り替え」をクリックします。 既に存在するものにこのコードを追加します。

```
approvalProcessID_Mod=notblank
approverStatuses:approvedByID=$$USER.ID
approverStatuses:approvedByID_Mod=in
```

## タスク — 少なくとも 1 つのプロジェクト間の先行タスクを持つすべてのタスクを表示する

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

## タスク — 自分が割り当てたすべてのタスクを表示する

任意のフィルターでタスクレポートを作成し、「フィルター」タブに移動して、「テキストモードに切り替え」をクリックします。 既に存在するものにこのコードを追加します。

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

ログインしたユーザーが現在の担当者の 1 つ以上を割り当てたすべてのタスクが表示されます。 担当者が複数の担当者によって割り当てられた場合は、担当者を最初に割り当てた人の名前のみがタスクのランディングページに「担当者」と表示されます。

## タスク — 完了したすべてのタスクを表示する — 承認待ち

```
status=CPL:A
status_Mod=in
```


## 問題 — 完了したすべての問題を表示する — 承認待ち

```
status=CPL:A
status_Mod=in
```


## プロジェクト — 完了したすべてのプロジェクトを表示する — 承認待ち

```
status=CPL:A
status_Mod=in
```


## 注意 — タグ付けされたすべてのコメントを表示する

```
tags:userID=$$USER.ID
tags:userID_Mod=in
```


## パラメータ/カスタムフィールドレポート — カスタムフォームに添付されていないカスタムフィールドを表示する（クリーンアップ作業で非常に役立つ）

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```
