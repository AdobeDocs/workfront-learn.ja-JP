---
title: リマインダー通知を設定
description: 作業の期限が近い、または期限切れになった時期をユーザーに知らせるための、オブジェクト固有のリマインダー通知を設定する方法を説明します。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner
thumbnail: setupremindnote.png
jira: KT-10091
exl-id: f1ba58d7-3226-4c62-8aa4-40f88495b833
source-git-commit: 4568e4e47b719e2dee35357d42674613112a9c43
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 100%

---

<!--
this has the same content as the system administrator notification setup and mangement section of the email and inapp notificiations learning path
-->

# リマインダー通知を設定

リマインダー通知は、システム管理者が[!UICONTROL 設定]エリアで作成します。プロジェクト、タスク、イシューの所有者が、作業の期限が近い、期限が切れている時期のリマインダーとして、リマインダー通知を添付して使用できます。

リマインダーはオブジェクト固有なので、通知を送信できるように、対応する作業項目に手動で添付する必要があります。

**リマインダー通知を作成**

1. **[!UICONTROL メインメニュー]**&#x200B;で「**[!UICONTROL 設定]**」をクリックします。
1. 「**[!UICONTROL メール]**」セクションをクリックします。
1. 「**[!UICONTROL 通知]**」セクションをクリックします。
1. 「**[!UICONTROL 新しいリマインダー]**」タブをクリックします。
1. 「**[!UICONTROL +新規リマインダー通知]**」ボタンをクリックします。
1. ドロップダウンメニューで目的のオブジェクトを選択します。
1. 必要な情報を入力します。
1. 「**[!UICONTROL 保存]**」をクリックします。

![[!UICONTROL 新規リマインダー通知]ウィンドウ](assets/admin-fund-reminder-notification-1.png)

リマインダーを設定する際に考慮すべき点を以下に示します。

* **[!UICONTROL リマインダー通知名] -**&#x200B;これは、プロジェクトマネージャがリマインダーをオブジェクトに付加する際に表示される名前です。名前は簡潔でわかりやすいものにしてください。
* **[!UICONTROL 対象期間] -**「タイミング」セクションで選択した日付の前後の時間、日、週、月の数。
* **[!UICONTROL タイミング] -**&#x200B;リマインダーを、オブジェクトの予定日、見込み日、実際の開始日／完了日の前後のどちらに送信するかを選択します。 タイムシートのオプションは、開始日、終了日、最終更新日に関連します。
* **[!UICONTROL 条件] -**&#x200B;送信するリマインダーを絞り込むための条件を指定します。オプションは、オブジェクト固有のリマインダーに応じて異なります。
* **[!UICONTROL 受信者] -**&#x200B;リマインダーの送信先を選択します。 関係者のオプションは、リマインダー用に選択したオブジェクトタイプに応じて異なります。

リマインダー設定を確立して保存すると、オブジェクト所有者は、[!DNL Workfront] 内でリマインダー通知を使用できるようになります。

## メールのカスタマイズ

リマインダー通知では、デフォルトのメール形式とメッセージが使用されます。 メールをカスタマイズする場合は、テンプレートを作成できます。

<!--
paragraph above needs a hyperlink to an article
-->

![新規メールテンプレートウィンドウ](assets/admin-fund-email-customization.png)

<!--
learn more URLs
-->
