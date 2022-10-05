---
title: システム監査ログの理解
description: システム監査ログを使用して、変更が行われたタイミングと項目を確認する方法を説明します。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner, Intermediate
thumbnail: 10040.jpeg
kt: 10040
exl-id: 9de6fd40-10fb-47a6-b186-3a38c411f1ac
source-git-commit: adf12d7846d2a1b4c32513a3955c080905044576
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---

# システム監査ログの理解

システム監査ログは、システム管理者が何が起こっているかを常に把握する最善の方法です [!DNL Workfront]. ログは、誰が何を変更し、いつ変更したかに関する真実の源と考えてください。

監査ログにアクセスするには、 [!UICONTROL 環境設定] セクション [!UICONTROL 設定] 領域 デフォルトでは、過去 7 日間のデータが表示されます。 様々な日付範囲のデータを表示するには、フィルター条件を変更します。

ユーザーが特定のアクションを実行した場合、 [!UICONTROL Workfront] は、 [!UICONTROL 監査ログ] セクション [!UICONTROL 設定] 領域

![[!UICONTROL ログタイプ] ドロップダウンメニュー [!UICONTROL 監査ログ] ページ内 [!UICONTROL 設定]](assets/admin-fund-audit-log-1.png)

記録された（ログに記録された）各アクションには、次の内容が表示されます。

* 変更の日時
* ログのタイプ
* アクションを完了したユーザーの名前
* オブジェクト
* アクションに関連付けられた詳細
* IP アドレス

![[!UICONTROL 監査ログ] リスト](assets/admin-fund-audit-log-2.JPG)

## 監査ログの書き出し

監査ログデータを書き出すと、システム管理者は、内部/外部の監査人やセキュリティスペシャリストと情報を共有できます。 一部の組織では、サイバーセキュリティ規制に準拠するために、特定のログの保持が必要です。 セキュリティシステムに読み込まれた情報を分析に使用する必要がある場合もあります。

監査ログは、CSV（コンマ区切り値）ファイルで書き出すことができます。このファイルは、スプレッドシートアプリケーションまたはプレーンテキストエディターで開くことができます。 エクスポートは一度に 50,000 行に制限されるので、合計が 50,000 を超える場合は、フィルターを使用してリストを絞り込みます。

![[!UICONTROL 書き出し] ボタン [!UICONTROL 監査ログ] ページ](assets/admin-fund-audit-log-3.png)

<!---
learn more URLs
Audit logs
Managing audit logs
--->
