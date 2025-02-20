---
title: グラフを使用したレポートの作成
description: グラフによるデータのビジュアライゼーションの改善方法と、Workfront でのグラフツールの使用方法を説明します。
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335153.png
jira: KT-8860
exl-id: ea3b360b-1fbd-4d1a-b505-b75759d24e41
doc-type: video
source-git-commit: 6afb57b983b094f9bc0c082a160453ecb394ca8e
workflow-type: ht
source-wordcount: '343'
ht-degree: 100%

---

# グラフを使用したレポートの作成

このビデオでは、以下について説明します。

* グラフによるデータのビジュアライゼーションの改善方法
* Workfront でのグラフツールの使用方法

>[!VIDEO](https://video.tv.adobe.com/v/335155/?quality=12&learn=on)

## グラフを使用したレポートの作成アクティビティ

このページの PDF をダウンロードするには、[こちらをクリック](/help/assets/create-reports-with-charts-activities.pdf)してください。

### アクティビティ 1：レポートへのグラフの追加

四半期の終わりが近づいており、最近完了したプロジェクトがどの程度予算内に収まっているかを確認します。プロジェクトの予定コストと実績コストを示すレポートを作成します。前四半期に完了したプロジェクトのみを表示します。カスタムのカラーを使用して、組み合わせの縦棒グラフを追加します。

### 回答 1

1. **[!UICONTROL メインメニュー]**&#x200B;から「**[!UICONTROL レポート]**」を選択します。
1. **[!UICONTROL 新しいレポート]**&#x200B;メニューをクリックし、「**[!UICONTROL プロジェクト]**」を選択します。
1. 「**[!UICONTROL 列（表示）]**」タブで、「**[!UICONTROL 列を追加]**」をクリックします。
1. [!UICONTROL プロジェクト]／[!UICONTROL 予定コスト]を選択し、この列を&#x200B;**[!UICONTROL 合計]**&#x200B;で集計します。
1. 「**[!UICONTROL 列を追加]**」を再度クリックします。
1. [!UICONTROL プロジェクト]／[!UICONTROL 実績コスト]を選択し、この列を&#x200B;**[!UICONTROL 合計]**&#x200B;で集計します。

   ![レポートに列を追加する画面の画像](assets/chart-report-columns.png)

1. 「**[!UICONTROL グループ化]**」タブで[!UICONTROL プロジェクト]／[!UICONTROL 名前]を選択し、レポートをグループ化するように設定します。

   ![レポートにグループ化を追加する画面の画像](assets/chart-report-groupings.png)

1. 「**[!UICONTROL フィルター]**」タブで、次の 2 つのフィルタールールを追加します。

   * [!UICONTROL プロジェクト]／[!UICONTROL ステータスが次と等しい]／[!UICONTROL 完了]
   * [!UICONTROL プロジェクト]／[!UICONTROL 実際の完了日]／[!UICONTROL 前四半期]

   ![レポートにフィルターを追加する画面の画像](assets/chart-report-filters.png)

1. 「**[!UICONTROL グラフ]**」タブで、グラフタイプとして「**[!UICONTROL 列]**」を選択します。
1. [!UICONTROL 左（Y）軸]については、[!UICONTROL プロジェクト]／[!UICONTROL 予定コスト]を選択します。
1. [!UICONTROL 下（X）軸]については、[!UICONTROL プロジェクト]／[!UICONTROL 名前]を選択します。
1. 「**[!UICONTROL 組み合わせグラフ]**」ボタンをクリックし、「**[!UICONTROL 値]**」フィールドで[!UICONTROL プロジェクト]／[!UICONTROL 実際のコスト]を選択します。
1. カラーボックスの横にある矢印をクリックし、[!UICONTROL 実際のコスト]のカラーを変更します。表示されるカラーの 1 つを選択するか、右下隅のボックスをクリックしてカラーパレットを表示します。
1. 「**[!UICONTROL 保存して閉じる]**」をクリックします。レポート名の入力を求められたら、「前四半期に完了したプロジェクトごとの予定コストと実際のコスト」と入力します。

   ![レポートにグラフを追加する画面の画像](assets/chart-report-chart.png)
