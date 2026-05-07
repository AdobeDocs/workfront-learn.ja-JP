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
hide: true
exl-id: 9986469c-b02f-48ac-b71e-055473a2855b
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T19:17:51.764Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
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
