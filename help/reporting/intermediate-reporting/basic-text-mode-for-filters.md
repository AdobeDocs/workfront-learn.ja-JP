---
title: フィルターの基本的なテキストモードについて
description: テキストモードとは何か、キャメルケースとは何か、Workfront のレポートフィルターで使用できる基本的な「プラグ＆プレイ」テキストモードについて説明します。
activity: use
feature: Text Mode Reporting
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: 2024-10-04T00:00:00Z
jira: KT-9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
doc-type: video
source-git-commit: 2c9e57b8f85c74061bd3e52ef4eaea60bc4ec5bb
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 98%

---

# フィルターの基本的なテキストモードについて

>[!PREREQUISITES]
>
>* [レポート要素について](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-elements.html?lang=ja)
>* [レポートコンポーネントについて](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-components.html?lang=ja)
>* [基本フィルターを作成](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/basic-text-mode-for-filters.html?lang=ja)


>[!TIP]
>
>* テキストモードをより深く理解するために、録画されたウェビナーイベント「[エキスパートに聞く - テキストモードレポートの概要](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=ja)」（所要時間：1 時間）の視聴をお勧めします。
>* テキストモードの詳細については、[詳細なレポート](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=ja)のチュートリアルをご覧ください。このチュートリアルは合わせて 5 時間半です。
>* ここをクリックして、[[!UICONTROL API エクスプローラー]](https://developer.adobe.com/workfront/api-explorer/)にアクセスします


このビデオでは、次のことを学習します。

* テキストモードとは
* キャメルケースとは
* レポートフィルターで使用できるいくつかの基本的な「プラグ＆プレイ」テキストモード

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12&learn=on)

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
