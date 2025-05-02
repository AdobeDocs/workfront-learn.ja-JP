---
title: システム監査ログについて
description: システム監査ログを使用して、変更が行われたタイミングとアイテムを確認する方法を説明します。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner, Intermediate
thumbnail: 10040.jpeg
jira: KT-10040
exl-id: 9de6fd40-10fb-47a6-b186-3a38c411f1ac
source-git-commit: 4568e4e47b719e2dee35357d42674613112a9c43
workflow-type: ht
source-wordcount: '265'
ht-degree: 100%

---

# システム監査ログについて

システム監査ログを使用すると、システム管理者は [!DNL Workfront] で何が起こっているかを常に把握できます。ログは、いつ誰が何を変更したかに関する、信頼できる情報源です。

[!UICONTROL 設定]エリアの[!UICONTROL 環境設定]セクションに移動して、監査ログにアクセスします。デフォルトでは、過去 7 日間のデータが表示されます。フィルター条件を変更すると、様々な日付範囲でデータを表示できます。

ユーザーが特定のアクションを実行すると、[!UICONTROL Workfront] は[!UICONTROL 設定]エリアの[!UICONTROL 監査ログ]セクションにそれらを記録します。

![設定の[!UICONTROL 監査ログ]ページのログタイプドロップダウンメニュー](assets/admin-fund-audit-log-1.png)

ログに記録された各アクションには、次の内容が表示されます。

* 変更の日時
* ログのタイプ
* アクションを実施したユーザーの名前
* オブジェクト
* アクションに関する詳細
* IP アドレス

![[!UICONTROL 監査ログ]リスト](assets/admin-fund-audit-log-2.JPG)

## 監査ログのエクスポート

監査ログデータをエクスポートすると、システム管理者は、内外の監査人やセキュリティスペシャリストと情報を共有できます。サイバーセキュリティ規則に準拠するために、特定のログを保持する必要がある組織もあります。情報をセキュリティシステムにインポートして分析する必要がある組織もあります。

監査ログは、CSV（コンマ区切り値）ファイルでエクスポートできます。このファイルは、スプレッドシートのアプリケーションやプレーンテキストのエディターで開くことができます。一度に書き出すことができるのは 50,000 レコードまでなので、合計が 50,000 レコードを超える場合は、フィルターを使用してリストを絞り込みます。

![[!UICONTROL 監査ログ]ページの「書き出し」ボタン](assets/admin-fund-audit-log-3.png)

<!--
learn more URLs
Audit logs
Managing audit logs
-->
