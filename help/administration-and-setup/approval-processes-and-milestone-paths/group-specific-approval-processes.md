---
title: グループ特有の承認プロセスについて
description: グループ管理者が管理対象のグループの承認プロセスをどのように作成または編集できるかについて説明します。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate
kt: 10017
exl-id: 138989b2-32d7-43e5-9660-d7b4172f232a
source-git-commit: 02bc5a09a838be6d98c9b746bff731236ee4116f
workflow-type: ht
source-wordcount: '212'
ht-degree: 100%

---

# グループ特有の承認プロセスについて

[!DNL Workfront] では、システム管理者とグループ管理者の両方が承認プロセスを作成できます。システム管理者は、[!DNL Workfront] システム全体で使用するプロセスや、特定のグループのみのプロセスを作成できます。グループ管理者は、管理対象のグループのプロセスのみを作成または編集できます。

[!DNL Workfront] で全員が使用できる承認プロセスの場合、必ず「[!UICONTROL この承認の利用者]」フィールドを[!UICONTROL すべてのグループ]に設定してください。

![[!UICONTROL グループフィールドがハイライトされた承認プロセスを編集]ウィンドウ](assets/admin-fund-approval-processes-1.png)

「[!UICONTROL ステータスが次のように設定された場合、承認プロセスを開始]」で使用できるステータスは、「この承認の利用者」フィールドでの選択によって異なります。[!UICONTROL すべてのグループ]が選択されている場合、システム全体でロックされているステータスのみを使用できます。

特定のグループの承認プロセスを制限するには、「[!UICONTROL この承認の利用者]」フィールドのリストからそのグループの名前を選択します。

![[!UICONTROL グループフィールドが展開された承認プロセスを編集]ウィンドウ](assets/admin-fund-approval-processes-2.png)

[!UICONTROL すべてのグループ]オプションは、グループ管理者に対しては使用できません。

特定のグループが選択されている場合、そのグループに対して使用できるステータスのみが、「[!UICONTROL ステータスが次のように設定された場合、承認プロセスを開始]」に表示されます。

![[!UICONTROL ステータスフィールドがハイライトされた承認プロセスを編集]ウィンドウ](assets/admin-fund-approval-processes-3.png)

