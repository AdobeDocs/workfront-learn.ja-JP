---
title: 複数の請求レートについて
description: プロジェクト内のシステム請求レートを上書きする方法を学びます。
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-multiple-billing-rates.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10048
hide: true
exl-id: 5b1ae2c4-43bd-4382-900f-078ef84408a5
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T19:00:23.025Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 438
ht-degree: 93%

---

# 複数の請求レートについて

プロジェクトマネージャーは [!DNL Workfront] 内で、特定のプロジェクト内のシステム請求レートを上書きすることができます。 以前は、新しい請求レートがプロジェクトに適用された場合、その請求レートが将来の時間に影響を与えるだけでなく、プロジェクトに既に記録されている時間にも影響がありました。

[!DNL Workfront]の新しい複数請求レート機能を使用すると、プロジェクトマネージャーは請求レートを適用する期間を決定できます。 このようにして、レートが交渉または変更された場合、プロジェクトマネージャはそのレートがいつ有効になるかを判断することができます。

## 請求レートの変更

1. プロジェクトのランディングページに移動します。 左側のパネルから「**[!UICONTROL 請求レート]**」を選択します。

   ![で[!UICONTROL 請求レート]を選択している画像[!DNL Workfront]](assets/project-finances-1.png)

1. 「**[!UICONTROL 請求レート]**」タブで、「**[!UICONTROL 請求レートを追加]**」ボタンをクリックします。 「**[!UICONTROL 新しい請求レート]**」をドロップダウンから選択します。

   ![で[!UICONTROL 新しい請求レート]を選択している画像[!DNL Workfront]](assets/project-finances-2.png)

1. [!UICONTROL 新しい請求レート]ダイアログボックスが表示されます。 **[!UICONTROL 担当業務]**&#x200B;ドロップダウンで、新しい請求レートを適用する担当業務を選択します。

   ![ の新しい請求レートで担当業務を選択している画像[!DNL Workfront]](assets/project-finances-3.png)

1. 担当業務が選択されると、[!UICONTROL デフォルトの請求レート]および[!UICONTROL 請求レート 1] フィールドが表示されます。 新しい請求レートを[!UICONTROL 請求レート 1] フィールドに入力します。 その請求レートがプロジェクト全体（記録された過去、現在、および未来の時間）に適用される場合は、「**[!UICONTROL 保存]**」ボタンをクリックします。

   ![ でプロジェクト全体に適用される新しい請求レートを保存している画像[!DNL Workfront]](assets/project-finances-5.png)

1. 新しい請求レートが特定の期間のみ適用される場合は、「**[!UICONTROL レートの追加]**」ボタンをクリックします。 [!UICONTROL 請求レート 1 の終了日]と[!UICONTROL 請求レート 2] フィールドが表示されます。 [!UICONTROL 請求レート 1] の終了日を入力します。 [!UICONTROL 請求レート 1] の開始日は入力できません。システムが、この請求レートはプロジェクトの最初に開始されたと想定しているからです。

   ![ で、プロジェクト開始から一定期間適用される新しい請求レートを作成している画像[!DNL Workfront]](assets/project-finances-6.png)

1. そうでない場合：

   * [!UICONTROL 請求レート 1] に、デフォルトの請求レートを入力します。
   * [!UICONTROL 請求レート 1]（[!UICONTROL デフォルトの請求レート]）の終了日を選択をします。
   * [!UICONTROL 請求レート 2] の開始日は、 [!UICONTROL 請求レート 1] 終了の翌日に、自動的に設定されます
   * [!UICONTROL 請求レート 2] セクションに希望の請求レートを入力します。
   * 必要な場合は「**[!UICONTROL 請求レートの追加]**」ボタンをクリックして、請求レートの追加を継続します。
   * 完了したら、「**[!UICONTROL 保存]**」をクリックします。
   * すべての請求レートが、プロジェクトの「[!UICONTROL 請求レート]」タブに表示されます。

   ![ で、異なる期間に適用される新しい請求レートを作成している画像。[!DNL Workfront]](assets/project-finances-7.png)
