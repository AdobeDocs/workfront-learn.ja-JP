---
title: かんばんチームとしての作業の管理
description: かんばんチームのページを通じて、作業とチームを管理する方法について説明します。
feature: Agile
role: Admin, Leader, User
level: Intermediate
jira: KT-10888
thumbnail: manage-work-kanban.png
exl-id: 05656ae0-46b2-4034-ac25-d936090d134c
TQID: 'https://experienceleague.adobe.com/-TulZuk86f5dTHLZahmcVIfVyyOIqDtE6NOr9brrOB0'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: be65ef36-43e4-48e1-a062-caa3778e15be
    internal-label: Agile
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
    internal-label: Leader
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
source-git-commit: 54883ad8c8df3aaee06ba8f8dca64227594c1c77
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 94%
---
# かんばんチームとしての作業の管理

かんばんチームとしての作業の管理
カンバンバックログへのストーリーの追加
Creativeマーケティング部門のバックログに、ストーリーを追加する方法はいくつかあります。

チームは、バックログから直接ストーリーを追加できます。
また、プロジェクトにタスクを割り当てることもできます。 クリエイティブマーケティングチームにルーティングされたリクエストがある場合、リクエストはチームの「リクエスト」タブに表示されます。 チームがリクエストを選択してストーリーに変換すると、これらはチームのバックログに表示されます。


## かんばんボードの使用

バックログのストーリーに優先順位を付けた後、かんばんボードに移動します。 そのストーリーに取り組むチームメンバーのアバターをストーリーカードにドラッグ＆ドロップすることで、割り当てを行うことができます。


ストーリーの進捗に応じて、チームはストーリーボードの適切なステータスに移動します。 チームメンバーは、かんばんフラグを使用して、ストーリーが順調か、ブロックされているか、取り込む準備が整っているかを示すことができます。 これにより、どの作業アイテムが順調に進んでいるか、作業の準備が整っているかどうかを他のチームメンバーに伝えることができます。

![かんばんカード](assets/kanban-01.png)

また、チームメンバーは、ストーリーボード上で直接カードを更新して、説明、ステータス、優先度などの変更を反映させることもできます。 これを行うには、ストーリーカードのドロップダウンメニューをクリックし、適切なフィールドを編集します [1]。

![かんばんカードのステータス](assets/kanban-02.png)

## かんばんストーリーの実行

あなたは処理中の作業の上限である 5 つのストーリーを使用しています。 ボードを見ると、タスクをステータス列に移動する際に、各レーンのタスク数が各ステータス列の右上に表示されていることがわかります。

![かんばんの WIP 制限](assets/kanban-03.png)

新規または処理中と同等のステータス列の上限を超えると、処理中の作業の上限を超えたことを示すエラーメッセージが表示されます。

![WIP 制限の超過](assets/kanban-04.png)

チームが一度に処理できるアイテムの数を増やせる／減らせると判断した場合、ユーザー（および編集権限を持つ他のチームメンバー）は、WIP 番号をクリックし、新しい決定を反映させるように編集することで、ストーリーボードから処理中の作業の数を直接変更できます。
