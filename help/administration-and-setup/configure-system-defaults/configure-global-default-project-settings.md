---
title: グローバルデフォルトプロジェクト設定の構成
description: カスタムステータスの変更、グローバルプロジェクト環境設定の設定、およびグローバル既定設定のスケジュールの作成方法を説明します。
feature: System Setup and Administration
role: Admin
level: Intermediate
activity: deploy
type: Tutorial
team: Technical Marketing
thumbnail: 335065.png
kt: 8753
exl-id: b961ba8c-9597-4ed4-a6d7-79689c8e290d
source-git-commit: adf12d7846d2a1b4c32513a3955c080905044576
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---

# グローバル既定のプロジェクト設定を構成する

<!---
21.4 updates have been made
--->

このビデオでは、次の方法を学習します。

* カスタムステータスの変更
* グローバルプロジェクト環境設定の指定
* スケジュールの作成と使用

>[!VIDEO](https://video.tv.adobe.com/v/335065/?quality=12)

## プロジェクト、タスク、問題の設定をグローバルおよびグループ化します

を開くと、 [!UICONTROL プロジェクト] の設定 [!DNL Workfront]「[!UICONTROL システムプロジェクト環境設定]」と入力します。 これにより、これらの設定が [!DNL Workfront] システム — グローバルな設定です。

![[!UICONTROL プロジェクト環境設定] ページ内 [!UICONTROL 設定]](assets/admin-fund-system-project-preferences-1.png)

同じようなものが [!UICONTROL タスクと問題] 設定。

![[!UICONTROL タスクと問題の環境設定] in [!UICONTROL 設定]](assets/admin-fund-task-issue-preferences-2.png)

しかし、 [!DNL Workfront] には、同じプロジェクト、タスクおよび問題の環境設定が必要です。 例えば、マーケティンググループが新しいプロジェクトのステータスを Planning にし、プロジェクトマネージャーグループが Request ステータスを優先するとします。

[!DNL Workfront] グループ管理者は、グループの特定のプロジェクト、タスクおよび問題の環境設定を調整できます。 どの環境設定を調整できるかは、 [!DNL Workfront] ロック/ロック解除を使用するシステム管理者がトグルを切り替えます。

最初に、 [!UICONTROL 設定] 領域：

1. 選択 **[!UICONTROL 設定]** 内 **[!UICONTROL メインメニュー]**.
1. 展開 **[!UICONTROL プロジェクト環境設定]** をクリックします。
1. 選択 **[!UICONTROL プロジェクト]** または **[!UICONTROL タスクと問題]**&#x200B;に設定されます。

グループ管理者がグループの設定を調整できないように、環境設定をロックします。

![ロックされた環境設定メッセージ](assets/admin-fund-preferences-locked-3.png)

環境設定のロックを解除して、グループ管理者がカスタマイズできるようにします。

![ロック解除済みの環境設定メッセージ](assets/admin-fund-preferences-unlocked-4.png)

一部の設定は、ロックを解除できず、グローバルシステム設定のままになります。

![ロックされた環境設定メッセージ](assets/admin-fund-preferences-always-locked-5.png)

### グループとサブグループの環境設定の指定

システム管理者がロックを解除した設定に対しては、グループ管理者は、管理するグループと、それらのグループの下にネストされたサブグループに対して調整を行うことができます。 また、グループ管理者は、グループ管理者が変更できる設定を管理できます。

1. 選択 **[!UICONTROL 設定]** 内 **[!UICONTROL メインメニュー]**.
1. クリック **[!DNL Groups]** をクリックします。
1. グループ名またはサブグループ名をクリックして開きます。
1. 選択 **[!UICONTROL プロジェクト環境設定]** または **[!UICONTROL タスクと問題の環境設定]** をクリックします。
1. ロックが解除された各環境設定に必要な変更を加えます。
1. 選択 **[!UICONTROL 保存]**.

![[!UICONTROL プロジェクトステータス] のセクション [!UICONTROL グループ] ページ](assets/admin-fund-group-preferences.png)

グループ管理者を使用していない場合、システム管理者は異なるグループの環境設定を管理できます。

<!---
learn more URLs and guides
Create or edit a group status 
Group administrators 
Configure system-wide project preferences 
Configure project preferences for a group 
Configure task and issue preferences for a group 
Create and modify a group’s schedule 
--->
