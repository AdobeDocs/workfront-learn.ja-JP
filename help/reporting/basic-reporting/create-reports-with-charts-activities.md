---
title: グラフアクティビティを使用したレポートの作成
description: ステップごとの手順を使用して、グラフを含むレポートを作成する練習を行います。
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335153.png
jira: KT-8860
hidefromtoc: true
source-git-commit: 915b28bbbf138fa84dce6d1915387fbe22c63362
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 81%

---

# グラフアクティビティを使用したレポートの作成

ステップごとの手順を使用して、グラフを含むレポートを作成する練習を行います。

## アクティビティ 1：レポートへのグラフの追加

四半期の終わりが近づいており、最近完了したプロジェクトがどの程度予算内に収まっているかを確認します。プロジェクトの予定コストと実績コストを示すレポートを作成します。前四半期に完了したプロジェクトのみを表示します。カスタムのカラーを使用して、組み合わせの縦棒グラフを追加します。

## 回答 1

1. **[!UICONTROL メインメニュー]**&#x200B;から&#x200B;**[!UICONTROL レポート]**&#x200B;を選択します。
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
1. 「**[!UICONTROL 保存して閉じる]**」をクリックします。レポート名の入力を求められたら、「前四半期に完了したプロジェクト別の予定コストと実際のコスト」と呼びます。

   ![レポートにグラフを追加する画面の画像](assets/chart-report-chart.png)
