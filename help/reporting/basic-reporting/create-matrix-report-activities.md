---
title: マトリックスレポートアクティビティの作成
description: ステップごとの手順を使用して、マトリックスレポートの作成を練習します。
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335156.png
jira: KT-8861
hidefromtoc: true
source-git-commit: 915b28bbbf138fa84dce6d1915387fbe22c63362
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 66%

---

# マトリックスレポートアクティビティの作成

ステップごとの手順を使用して、マトリックスレポートの作成を練習します。

## アクティビティ 1：マトリックスレポートの作成

各ステータスのリクエスト数をリクエストキューで並べ替えたマトリックスレポートを作成します。これにより、流入する作業量と、それに対してどの程度対応できているかをスナップショットで簡単に把握できます。

リクエストキューをレコードのグループ化に表示します。ステータスを、列のグループ化として表示します。レポートに「ステータスとリクエストキュー別のリクエスト」という名前を付けます。

## 回答 1

1. **[!UICONTROL メインメニュー]**&#x200B;から&#x200B;**[!UICONTROL レポート]**&#x200B;を選択します。
1. 「**[!UICONTROL 新しいレポート]**」オプションをクリックし、「**[!UICONTROL イシュー]**」を選択します。
1. 「**[!UICONTROL グループ化]**」タブに移動し、「**[!UICONTROL マトリックスグループ化に切り替え]**」をクリックします。
1. [!UICONTROL レコードのグループ化]の場合は、**[!UICONTROL プロジェクト]**／**[!UICONTROL 名前]**&#x200B;を選択します。
1. [!UICONTROL 列のグループ化]の場合は、**[!UICONTROL イシュー]**／**[!UICONTROL ステータス]**&#x200B;を選択します。

   ![新しいイシューレポートのグループ化を作成する画面の画像](assets/matrix-report-groupings.png)

1. 「**[!UICONTROL フィルター]**」タブに移動します。
1. アクティブなリクエストキューのリクエストのみが表示されるようにするには、次のフィルタールールを追加します。

   * [!UICONTROL プロジェクト]／[!UICONTROL ステータスが次と等しい]／[!UICONTROL 次と等しい]／[!UICONTROL 現在]
   * [!UICONTROL キュー定義]／[!UICONTROL 公開済み]／[!UICONTROL 等しくない]／[!UICONTROL なし]（このようにして、プロジェクトが実際にはリクエストキューであることがわかります。キュー定義は、公開オプションの 1 つに割り当てられます）。

1. 「**[!UICONTROL 保存して閉じる]**」をクリックします。レポート名の入力を求められたら、「ステータスとリクエストキューによるリクエスト」と入力します。

   ![新しいイシューレポートフィルターを作成する画面の画像](assets/matrix-report-filters.png)
