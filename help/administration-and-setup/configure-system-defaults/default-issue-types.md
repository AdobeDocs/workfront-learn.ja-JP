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
source-git-commit: 4568e4e47b719e2dee35357d42674613112a9c43
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 100%

---

# 既定のイシューステータスについて

各イシュータイプは異なるタイプの情報をトラッキングするので、イシューを解決するにはタイプごとに一意のワークフローが必要になる場合があります。各イシュータイプのステータスを、そのイシュータイプのワークフローに合わせてカスタマイズします。

<!--
add URL in paragraph below
-->

## 既定の状態

既定のイシューステータスには次の 4 つがあり、これらは削除できません。

* 新規
* 処理中
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


イシューのステータスは、[!UICONTROL 問題の詳細]で表示および変更できます。イシューのステータスは、右端にある問題ページのヘッダーで変更することもできます。

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
