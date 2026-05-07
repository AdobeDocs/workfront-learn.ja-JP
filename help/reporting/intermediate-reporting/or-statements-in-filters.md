---
title: フィルターでの OR ステートメントの作成
description: Workfront の柔軟なフィルターロジックを使用すると、デフォルトの「AND」ルール、オプションの「OR」条件、複雑な条件に対応する整理されたフィルターグループを使用して、レポートビューを絞り込むことができます。
activity: use
team: Technical Marketing
feature: Reports and Dashboards
thumbnail: create-or-statements-in-filters.png
type: Tutorial
role: User
level: Intermediate
jira: KT-9987
exl-id: 1a56f2f6-12df-43a5-943c-986a85661efa
last-substantial-update: '2025-08-11T00:00:00.000Z'
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-06T02:11:54.379Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 318
ht-degree: 65%

---

# フィルターでの OR ステートメントの作成

このビデオでは、Workfrontで複数のルールを持つフィルターを作成して使用する方法を説明します。 &#x200B; デフォルトでは、Workfrontはフィルタールールの間に「AND」を使用します。つまり、リストにアイテムが表示されるためには、すべての条件がtrueである必要があります。
または、フィルターロジックを「OR」に変更して、いずれかの条件を満たす項目を表示することもできます。
このビデオでは、フィルターグループを使用してタスクのフィルターを作成する方法も示しています。 &#x200B;例えば、2つのグループを作成できます。1つは、クリエイティブチームに割り当てられた不完全なタスクを遅らせるグループで、もう1つは、未割り当てのクリエイティブチームに割り当てられた不完全なタスクです。 &#x200B;各グループ内では、「AND」ロジックが適用されます。つまり、グループ内のすべての条件を満たす必要があります。 &#x200B; グループ間の「OR」ロジックにより、いずれかのグループの条件を満たすタスクが表示されます。

>[!VIDEO](https://video.tv.adobe.com/v/3470692/?quality=12&learn=on&enablevpops=0)

## OR フィルターアクティビティ

自分に割り当てられているまたは他のユーザーに割り当てられていない、不完全なタスクを検索します。 次のようなフィルターを設定します。 このフィルターで必要な結果が得られますか？ できる場合と、できない場合の理由を教えてください。

![不適切に作成された OR ステートメントの画像：[!DNL Workfront]](assets/or-statement-your-turn-1.png)

### 解答

いいえ。このフィルターではタスクの完了性のフィルタールールが OR の片側でしか設定されていないので、必要な結果（自分に割り当てられているか、誰にも割り当てられていない未完了のタスク）を得ることはできません。

代わりに、このフィルターでは、以下を示すリストが生成されます。

* 自分に割り当てられた未完了のタスク。
* **+（OR）**
* すべての未割り当てタスク（ステータスに関係なく）。

フィルターは次のようになります。 このフィルターでは、OR の両側でタスクの完了性のフィルタールールが設定されています。

![[!DNL Workfront]](assets/or-statement-your-turn-2.png) で適切に作成された OR ステートメントの画像
