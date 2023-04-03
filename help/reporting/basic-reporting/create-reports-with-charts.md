---
title: グラフを使用したレポートの作成
description: グラフでデータのビジュアライゼーションを改善する方法と、Workfrontのグラフツールの使用方法を説明します。
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335153.png
kt: 8860
exl-id: ea3b360b-1fbd-4d1a-b505-b75759d24e41
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 8%

---

# グラフを使用したレポートの作成

このビデオでは、以下について説明します。

* グラフによるデータのビジュアライゼーションの改善方法
* Workfrontのグラフツールの使用方法

>[!VIDEO](https://video.tv.adobe.com/v/335155/?quality=12&learn=on)

## アクティビティ：レポートへのグラフの追加

四半期の終わりが近づいており、完了したプロジェクトが予算にとどまった最近の状況を確認できます。 プロジェクトの計画原価と実際原価を示すレポートを作成します。 前の四半期に完了したプロジェクトのみを表示したい場合。 カスタムの色を使用して、組み合わせの縦棒グラフを追加します。

## 回答

1. **[!UICONTROL メインメニュー]**&#x200B;から&#x200B;**[!UICONTROL レポート]**&#x200B;を選択します。
1. 次をクリック： **[!UICONTROL 新しいレポート]** メニューと選択 **[!UICONTROL プロジェクト]**.
1. 内 **[!UICONTROL 列（表示）]** タブ、クリック **[!UICONTROL 列を追加]**.
1. 選択 [!UICONTROL プロジェクト] > [!UICONTROL 計画コスト] この列を以下のように要約します。 **[!UICONTROL 合計]**.
1. 「**[!UICONTROL 列を追加]**」を再度クリックします。
1. 選択 [!UICONTROL プロジェクト] > [!UICONTROL 実費] この列を以下のように要約します。 **[!UICONTROL 合計]**.

   ![レポートに列を追加する画面の画像](assets/chart-report-columns.png)

1. 内 **[!UICONTROL グループ化]** 」タブで、次の項目でグループ化するレポートを設定します。 [!UICONTROL プロジェクト] > [!UICONTROL 名前].

   ![グループ化をレポートに追加する画面の画像](assets/chart-report-groupings.png)

1. 内 **[!UICONTROL フィルター]** タブに次の 2 つのフィルタールールを追加します。

   * [!UICONTROL プロジェクト] > [!UICONTROL ステータスが次と等しい] > [!UICONTROL 完了]
   * [!UICONTROL プロジェクト] >[!UICONTROL  実際の完了日] > [!UICONTROL 前四半期]

   ![レポートにフィルターを追加する画面の画像](assets/chart-report-filters.png)

1. 内 **[!UICONTROL グラフ]** タブ、選択 **[!UICONTROL 列]** グラフのタイプを表します。
1. の [!UICONTROL 左 (Y) 軸]選択 [!UICONTROL プロジェクト] > [!UICONTROL 計画コスト].
1. の [!UICONTROL 下 (X) 軸]選択 [!UICONTROL プロジェクト] > [!UICONTROL 名前].
1. 次をクリック： **[!UICONTROL 組み合わせグラフ]** ボタンと選択 [!UICONTROL プロジェクト] > [!UICONTROL 実費] 内 **[!UICONTROL 値]** フィールドに入力します。
1. 色ボックスの横にある矢印をクリックして、 [!UICONTROL 実費] 色 表示される色の 1 つを選択するか、右下隅のボックスをクリックしてカラーパレットを表示します。
1. 「**[!UICONTROL 保存して閉じる]**」をクリックします。レポート名の入力を求められたら、「プロジェクト完了前四半期の計画原価と実績原価」と呼びます。

   ![レポートにグラフを追加する画面の画像](assets/chart-report-chart.png)
