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
kt: 10048
exl-id: bda562b9-f8da-49c9-bea7-0440fdc4c24c
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: ht
source-wordcount: '427'
ht-degree: 100%

---

# 複数の請求レートについて

プロジェクトマネージャーは [!DNL Workfront] 内で、特定のプロジェクト内のシステム請求レートを上書きすることができます。以前は、新しい請求レートがプロジェクトに適用された場合、その請求レートが将来の時間に影響を与えるだけでなく、プロジェクトに既に記録されている時間にも影響がありました。

[!DNL Workfront] の新しい複数請求レート機能を使用すると、プロジェクトマネージャーは請求レートを適用する期間を決定することができます。このようにして、レートが交渉または変更された場合、プロジェクトマネージャはそのレートがいつ有効になるかを判断することができます。

## 請求レートの変更

1. プロジェクトのランディングページに移動します。 左側のパネルから「**[!UICONTROL 請求レート]**」を選択します。

   ![で[!UICONTROL 請求レート]を選択している画像[!DNL Workfront]](assets/project-finances-1.png)

1. 「**[!UICONTROL 請求レート]**」タブで、「**[!UICONTROL 請求レートを追加]**」ボタンをクリックします。 「**[!UICONTROL 新しい請求レート]**」をドロップダウンから選択します。

   ![で[!UICONTROL 新しい請求レート]を選択している画像[!DNL Workfront]](assets/project-finances-2.png)

1. [!UICONTROL 新しい請求レート]ダイアログボックスが表示されます。 **[!UICONTROL 担当業務]**&#x200B;ドロップダウンで、新しい請求レートを適用する担当業務を選択します。

   ![ の新しい請求レートで担当業務を選択している画像[!DNL Workfront]](assets/project-finances-3.png)

1. 担当業務が選択されると、[!UICONTROL デフォルトの請求レート]および[!UICONTROL 請求レート 1] フィールドが表示されます。新しい請求レートを[!UICONTROL 請求レート 1] フィールドに入力します。 その請求レートがプロジェクト全体（記録された過去、現在、および未来の時間）に適用される場合は、「**[!UICONTROL 保存]**」ボタンをクリックします。

   ![ でプロジェクト全体に適用される新しい請求レートを保存している画像[!DNL Workfront]](assets/project-finances-5.png)

1. 新しい請求レートが特定の期間のみ適用される場合は、「**[!UICONTROL レートの追加]**」ボタンをクリックします。 [!UICONTROL 請求レート 1 の終了日]と[!UICONTROL 請求レート 2] フィールドが表示されます。 [!UICONTROL 請求レート 1] の終了日を入力します。[!UICONTROL 請求レート 1] の開始日は入力できません。システムが、この請求レートはプロジェクトの最初に開始されたと想定しているからです。

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
