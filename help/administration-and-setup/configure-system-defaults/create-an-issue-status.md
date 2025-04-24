---
title: イシューステータスの作成
description: 組織のワークフローのニーズに合わせてイシューステータスを作成する方法を説明します。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10019
exl-id: 1689080d-1d3c-4fad-a353-64fb3b0d5851
source-git-commit: 4568e4e47b719e2dee35357d42674613112a9c43
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# イシューステータスの作成

[!DNL Workfront] では、新しいステータスの作成を始める前に、システム内の既存のイシューステータスを修正することを推奨しています。これにより、維持する必要のあるステータスの数を制限できます。

1. **[!UICONTROL メインメニュー]**&#x200B;で「**[!UICONTROL 設定]**」をクリックします。
1. 左側のメニューパネルで「**[!UICONTROL プロジェクト環境設定]**」セクションを展開します。
1. 「**[!UICONTROL ステータス]**」を選択します。
1. 「**[!UICONTROL イシュー]**」タブを選択します。
1. 右上のフィールドが「[!UICONTROL システムステータス]」に設定されていることを確認します。これにより、新しいステータスが [!DNL Workfront] インスタンス全体でグローバルに利用できるようになります。
1. 「**[!UICONTROL マスターリスト]**」を選択すると、すべてのイシューのステータスが表示されます。ここで、ステータスを作成または変更します。
1. 「**[!UICONTROL 新しいステータスを追加]**」をクリックします。
1. 組織での必要に応じて、名前、説明、カラー、次と等しい、キーなどのフィールドを入力します。
1. このステータスを使用できるイシューのタイプのチェックボックスをオンにします。
1. 「**[!UICONTROL 保存]**」をクリックします。

![[!UICONTROL ステータス]ページの新しいステータスウィンドウ](assets/admin-fund-create-issue-status.png)

## イシューのステータスとグループ管理者

グループ管理者は、自分が管理するグループのイシューステータスを作成し、カスタマイズできます。これにより、グループの自立性が高まり、作業を継続するために必要なステータスが提供されます。また、システム全体のステータスを示す長いリストを作成する必要もありません。

システム管理者からカスタマイズできる権限を付与されている場合、グループ管理者は既存のステータスを編集できます。

システム管理者は、「[!UICONTROL ステータス]」ウィンドウの右上隅にあるグループ名を選択することで、グループのステータスを管理できます。

![[!UICONTROL ステータス]ページのグループリストメニュー](assets/admin-fund-change-group-master-list.png)

グループ管理者は、「[!UICONTROL 設定]」領域の「[!UICONTROL グループ]」セクションをクリックし、名前をクリックしてグループを開くと、左パネルのメニューで「[!UICONTROL ステータス]」を選択できます。必ず「イシュー」タブを選択します。

![[!UICONTROL グループ]ページの「ステータス」セクション](assets/admin-fund-group-issue-statuses.png)

<!--
For detailed information on how managing statuses can be done by group administrators, see these articles:
Create and customize group statuses
Group administrators
-->

<!--
learn more URLs
Issue statuses
Create and customize system-wide statuses
-->
