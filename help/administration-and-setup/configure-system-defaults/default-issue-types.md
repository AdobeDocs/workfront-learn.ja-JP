---
title: 既定のイシューステータスについて
description: 既定のイシューステータスと、それらを組織のワークフローに合わせてカスタマイズする理由について説明します。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10031
exl-id: ccdbba55-c409-44ac-b3d5-908f1637e19f
TQID: https://experienceleague.adobe.com/LfIPSU0xUwuqadnMUQ3BYm2-LR5FmEeOPLTgFLJ9p40
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 186
ht-degree: 100%

---

# 既定のイシューステータスについて

各イシュータイプは異なるタイプの情報をトラッキングするので、イシューを解決するにはタイプごとに一意のワークフローが必要になる場合があります。 各イシュータイプのステータスを、そのイシュータイプのワークフローに合わせてカスタマイズします。

<!--
add URL in paragraph below
-->

## 既定の状態

既定のイシューステータスには次の 4 つがあり、これらは削除できません。

* 新規
* 進行状況
* クローズ
* 保留中

[!DNL Workfront] には、その他に、イシュー管理に共通する次の 6 つの状態があります。

* 再オープン
* フィードバック待ち
* 複製不可
* 解決済み
* 完了確認
* 解決しない

<!--
need URL in paragraph below
-->


イシューのステータスは、[!UICONTROL 問題の詳細]で表示および変更できます。 イシューのステータスは、右端にある問題ページのヘッダーで変更することもできます。

![ページヘッダーと[!UICONTROL 問題の詳細]ページの「状態」オプション](assets/admin-fund-issue-details-status.png)

[!UICONTROL 状態]列をビューまたはカスタムレポートに追加すると、スムーズに表示および変更できるようになります。

![[!UICONTROL ビューの状態列]](assets/admin-fund-issue-status-view.png)

<!--
link the bullets below to the articles
-->

イシューのステータスの基本事項は次のとおりです。

* 既存の状態の変更
* システムの既定の状態
* 新しい状態の作成
