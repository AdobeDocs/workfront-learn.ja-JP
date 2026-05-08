---
title: グループ特有の承認プロセスについて
description: グループ管理者が管理対象のグループの承認プロセスをどのように作成または編集できるかについて説明します。
feature: Approvals
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate
jira: KT-10017
exl-id: 138989b2-32d7-43e5-9660-d7b4172f232a
TQID: https://experienceleague.adobe.com/PcQL0NTo4cz4jEOXcQ-48tXu8Zr5U-BsbAx9hKn20Tk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 214
ht-degree: 100%

---

# グループ特有の承認プロセスについて

[!DNL Workfront] では、システム管理者とグループ管理者の両方が承認プロセスを作成できます。 システム管理者は、[!DNL Workfront] システム全体で使用するプロセスや、特定のグループのみのプロセスを作成できます。 グループ管理者は、管理対象のグループのプロセスのみを作成または編集できます。

[!DNL Workfront] で全員が使用できる承認プロセスの場合、必ず「[!UICONTROL この承認プロセスの利用者]」フィールドを[!UICONTROL すべてのグループ]に設定してください。

![[!UICONTROL グループフィールドがハイライトされた承認プロセスを編集]ウィンドウ](assets/admin-fund-approval-processes-1.png)

「[!UICONTROL ステータスが次のように設定された場合、承認プロセスを開始]」メニューで使用できるステータスは、「利用者」フィールドでの選択によって異なります。 [!UICONTROL すべてのグループ]が選択されている場合、システム全体でロックされているステータスのみを使用できます。

特定のグループの承認プロセスを制限するには、「[!UICONTROL この承認プロセスの利用者]」フィールドのリストからそのグループの名前を選択します。

![[!UICONTROL グループフィールドが展開された承認プロセスを編集]ウィンドウ](assets/admin-fund-approval-processes-2.png)

[!UICONTROL すべてのグループ]オプションは、グループ管理者に対しては使用できません。

特定のグループが選択されている場合、そのグループに対して使用できるステータスのみが、「[!UICONTROL ステータスが次のように設定された場合、承認プロセスを開始]」メニューに表示されます。

![[!UICONTROL ステータスフィールドがハイライトされた承認プロセスを編集]ウィンドウ](assets/admin-fund-approval-processes-3.png)

