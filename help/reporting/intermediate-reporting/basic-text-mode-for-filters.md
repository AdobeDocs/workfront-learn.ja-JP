---
title: Workfrontのフィルターの基本的なテキストモードについて説明します
description: Workfront のレポートフィルターで使用できるテキストモード、キャメルケース、基本的なテキストモードについて学習します。
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: '2025-07-30T00:00:00.000Z'
jira: KT-9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
subfeature_v2:
  - id: cec4c78b-dd2b-46ec-b824-6ca30f0eb7b2
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-06T13:59:16.164Z'
source-git-commit: f0f541bf3fd6db69e6d813cf81456a5df6848d49
workflow-type: tm+mt
source-wordcount: 504
ht-degree: 95%

---

# Workfrontのフィルターの基本的なテキストモードについて説明します

>[!PREREQUISITES]
>
>* [Workfront レポートの要素を確認](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-elements.html?lang=ja)
>* [Workfrontのレポートコンポーネントを見る](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-components.html?lang=ja)
>* [基本フィルターを作成](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/basic-text-mode-for-filters.html?lang=ja)


>[!TIP]
>
>* テキストモードをより深く理解するために、録画されたウェビナーイベント「[エキスパートに聞く - テキストモードレポートの概要](https://experienceleague.adobe.com/en/docs/events/classics/reporting-and-dashboards/introduction-to-text-mode-reporting)」（所要時間：1 時間）の視聴をお勧めします。
>* テキストモードの詳細については、[詳細なレポート](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=jp)のチュートリアルをご覧ください。このチュートリアルは合わせて 5 時間半です。
>* ここをクリックして、[[!UICONTROL API エクスプローラー]](https://developer.adobe.com/workfront/api-explorer/)にアクセスします


このビデオでは、以下について説明します。

* テキストモード
* キャメルケース
* レポートフィルターで使用できるいくつかの&#x200B;_テキストモードのコードブロック_

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12&learn=on&enablevpops=0)

## 「フィルターの基本的なテキストモードについて」アクティビティ


### タスク -「自分の担当部分を完了」とマークしたタスクをフィルタリングで除外します

次のテキストモードでは、ユーザーが「自分の担当部分を完了」とマークしたタスクが除外されます。 必要な操作は、タスクフィルターを作成し、必要なフィルタールールを追加してから、テキストモードに切り替えて、フィルターに表示されるテキストモードの後に以下のコードをペーストするだけです。


>[!WARNING]
>
> これは、カレンダーフィルターでの使用は意図されていません。

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

### タスク - 承認待ちのすべてのタスクの表示

```
approvalProcessID_Mod=notblank
currentUserApproversMM:ID=$$USER.ID
currentUserApproversMM:ID_Mod=in
currentUserApproversMM_Join=allowingnull
```

### タスク - 承認したすべてのタスクの表示

必要なフィルターを使用してタスクレポートを作成し「フィルター」タブに移動して、「テキストモードに切り替える」をクリックします。 既に存在するものにこのコードを追加します。

```
approvalProcessID_Mod=notblank
approverStatuses:approvedByID=$$USER.ID
approverStatuses:approvedByID_Mod=in
```

### タスク - 少なくとも 1 つのクロスプロジェクトの先行タスクを持つすべてのタスクの表示

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

### タスク - 他のユーザーに割り当てたすべてのタスクの表示

必要なフィルターを使用してタスクレポートを作成し「フィルター」タブに移動して、「テキストモードに切り替える」をクリックします。 既に存在するものにこのコードを追加します。

>[!WARNING]
> 
> これは、カレンダーフィルターでの使用は意図されていません。

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

これにより、ログインしたユーザーが現在の担当者の少なくとも 1 人を割り当てたすべてのタスクが表示されます。 担当者が複数の人物によって割り当てられた場合、最初に誰かを割り当てたユーザーの名前のみが、タスクのランディングページに「リクエストしたユーザー」として表示されます。

### タスク - 完了 - 承認待ちのすべてのタスクの表示

```
status=CPL:A
status_Mod=in
```


### イシュー - 完了 - 承認待ちのすべてのイシューの表示

```
status=CPL:A
status_Mod=in
```


### プロジェクト - 完了 - 承認待ちのすべてのプロジェクトの表示

```
status=CPL:A
status_Mod=in
```


### メモ - タグ付けされたすべてのコメントの表示

```
tags:userID=$$USER.ID
tags:userID_Mod=in
```


### パラメーター／カスタムフィールドレポート - カスタムフォームに添付されていないカスタムフィールドの表示（クリーンアップ作業で非常に役立ちます）

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```
