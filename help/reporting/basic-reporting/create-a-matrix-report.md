---
title: マトリックスレポートの作成
description: マトリックスレポートが役立つタイミングと、Workfrontでマトリックスレポートを作成する方法について説明します。
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335156.png
kt: 8861
exl-id: e893d94a-e808-4bc1-bc6e-f46a5582b55d
source-git-commit: 252ba3ba44f22519a35899fcda9c6bca597a6c2c
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# マトリックスレポートの作成

このビデオでは、次のことを学習します。

* マトリックスレポートが役立つ場合
* マトリックスレポートの作成方法

>[!VIDEO](https://video.tv.adobe.com/v/335156/?quality=12)

## アクティビティ：マトリックスレポートの作成

各ステータスにあるリクエストの数をリクエストキューで並べ替えたマトリックスレポートを作成します。 これにより、入手される作業量と、それに対してどの程度適合しているかを簡単にスナップショットできます。

行グループにリクエストキューを表示する場合。 ステータスは列のグループ化として表示されます。 レポートに「Requests by Status and Request Queue」という名前を付けます。

## 回答

1. 選択 **[!UICONTROL レポート]** から **[!UICONTROL メインメニュー]**.
1. 次をクリック： **[!UICONTROL 新しいレポート]** オプションと選択 **[!UICONTROL 問題]**.
1. 次に移動： **[!UICONTROL グループ化]** タブをクリックし、 **[!UICONTROL マトリックスグループ化に切り替え]**.
1. の場合 [!UICONTROL 行のグループ化]を選択します。 **[!UICONTROL プロジェクト]** > **[!UICONTROL 名前]**.
1. の場合 [!UICONTROL 列のグループ化]を選択します。 **[!UICONTROL 問題]** > **[!UICONTROL ステータス]**.

   ![新しい問題レポートのグループ化を作成する画面の画像](assets/matrix-report-groupings.png)

1. 次に移動： **[!UICONTROL フィルター]** タブをクリックします。
1. アクティブなリクエストキューにリクエストのみが表示されるようにするには、次のフィルタールールを追加します。

   * [!UICONTROL プロジェクト] > [!UICONTROL ステータスが次と等しい] > [!UICONTROL 次と等しい] > [!UICONTROL 現在]
   * [!UICONTROL キュー定義] > [!UICONTROL 公開済み] > [!UICONTROL 等しくない] > [!UICONTROL なし] （このようにして、プロジェクトが実際にはリクエストキューであることがわかります。キュー定義は、パブリックオプションの 1 つに割り当てられます）。

1. クリック **[!UICONTROL 保存して閉じる]**. レポート名の入力を求められたら、「Requests by Status and Request Queue」と入力します。

   ![新しい問題レポートフィルターを作成する画面の画像](assets/matrix-report-filters.png)
