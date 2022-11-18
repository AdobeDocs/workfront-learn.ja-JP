---
title: 複数の請求率について
description: プロジェクト内のシステム請求率を上書きする方法を説明します。
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
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# 複数の請求率について

内 [!DNL Workfront]を使用すると、プロジェクトマネージャーは、特定のプロジェクト内のシステム請求率を上書きできます。 以前は、新しい請求率がプロジェクトに適用された場合、その請求は将来の時間に影響を与えるだけでなく、プロジェクトに既にログオンしている時間にも影響を与えていました。

を使用 [!DNL Workfront]の新しい複数請求レート機能により、プロジェクトマネージャーは請求レートを適用する期間を決定できます。 このようにして、レートがネゴシエートまたは変更された場合、プロジェクトマネージャはそのレートを有効にするタイミングを決定できます。

## 請求率の変更

1. プロジェクトのランディングページに移動します。 選択 **[!UICONTROL 請求率]** を左側のパネルからクリックします。

   ![選択の画像 [!UICONTROL 請求率] in [!DNL Workfront]](assets/project-finances-1.png)

1. 次の **[!UICONTROL 請求率]** タブで、 **[!UICONTROL 請求率を追加]** 」ボタンをクリックします。 選択 **[!UICONTROL 新しい請求率]** をドロップダウンから選択します。

   ![選択の画像 [!UICONTROL 新しい請求率] in [!DNL Workfront]](assets/project-finances-2.png)

1. この [!UICONTROL 新しい請求率] ダイアログボックスが表示されます。 次の **[!UICONTROL ジョブの役割]** ドロップダウンで、新しい請求率を適用するジョブロールを選択します。

   ![新しい請求率でジョブの役割を選択する画像 ( [!DNL Workfront]](assets/project-finances-3.png)

1. ジョブの役割を選択すると、 [!UICONTROL デフォルトの請求率] そして [!UICONTROL 請求率 1] フィールドが表示されます。 新しい請求率を [!UICONTROL 請求率 1] フィールドに入力します。 その請求率がプロジェクト全体（過去、現在および将来のログに記録された時間）に適用される場合は、 **[!UICONTROL 保存]** 」ボタンをクリックします。

   ![新しい請求率を保存する画像 ( [!DNL Workfront]](assets/project-finances-5.png)

1. 新しい請求率が特定の期間のみ適用される場合は、 **[!UICONTROL 追加率]** 」ボタンをクリックします。 この [!UICONTROL 請求レート 1 終了日] そして [!UICONTROL 請求率 2] フィールドが表示されます。 終了日を入力 [!UICONTROL 請求率 1]. 開始日は入力できません [!UICONTROL 請求率 1] システムは、プロジェクトの最初に開始されたと想定しているからです。

   ![特定の期間に適用される新しい請求率を作成する画像 ( [!DNL Workfront]](assets/project-finances-6.png)

1. そうでない場合：

   * のデフォルトの請求率を入力 [!UICONTROL 請求率 1].
   * 終了日を選択 [!UICONTROL 請求率 1] ([!UICONTROL デフォルトの請求率]) をクリックします。
   * 開始日： [!UICONTROL 請求率 2] は次の日の後に自動的に設定されます [!UICONTROL 請求率 1] 終了
   * 目的の請求率を [!UICONTROL 請求率 2] 」セクションに入力します。
   * 必要に応じて、 **[!UICONTROL 追加率]** 」ボタンをクリックします。
   * 完了したら、「 **[!UICONTROL 保存]**.
   * すべての請求率が [!UICONTROL 請求率] 」タブをクリックします。
   ![新しい請求率を作成する画像。 [!DNL Workfront]](assets/project-finances-7.png)
