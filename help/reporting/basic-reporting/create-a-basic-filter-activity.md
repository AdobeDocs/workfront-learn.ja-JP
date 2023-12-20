---
title: 基本フィルターアクティビティの作成
description: このアクティビティで、「今月を閉じる自分のプロジェクト」という名前のプロジェクトフィルターを作成します。
activity: use
feature: Reports and Dashboards
thumbnail: 336807.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8856
exl-id: fc29b4ce-2937-478e-abd5-0b559657ead0
doc-type: video
source-git-commit: 0ff5accae867f07cc31ac2be7b0c12981412346e
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 32%

---

# 基本フィルターアクティビティの作成

## アクティビティ 1 — マーケティングポートフォリオ内のすべてのプロジェクト

このアクティビティで、「マーケティングポートフォリオ内のすべてのプロジェクト」という名前のプロジェクトフィルターを [!UICONTROL レガシーフィルター] エクスペリエンス。 これにより、ステータスに関係なく、「マーケティングPortfolio」という名前のポートフォリオ内のすべてのプロジェクトが表示されます。

詳細な手順の説明がページの後半にあります。

### アクティビティ 1 に対する回答

![新しいフィルターを作成する画面の画像](assets/basic-filter-activity-1.png)

1. [!UICONTROL メインメニュー]から[!UICONTROL プロジェクト]エリアに移動します。プロジェクトのリストが表示されます。
1. 次をクリック： **[!UICONTROL フィルター]** メニューと選択 [!UICONTROL レガシーフィルター].
1. 選択 **[!UICONTROL 新しいフィルター]**.
1. フィルターに「All projects in the Marketing portfolio」という名前を付けます。
1. 「**[!UICONTROL フィルタールールを追加]**」をクリックします。
1. Adobe Analytics の [!UICONTROL フィールド名の入力を開始] フィールドに、&quot;と入力します。[!UICONTROL ポートフォリオ名]&quot;. 次に、 [!UICONTROL 名前] の下に [!UICONTROL Portfolio] フィールドのソース。
1. 「[!UICONTROL 次と等しい]」演算子はそのままにしておきます。
1. 「 」を入力します。[!UICONTROL マーケティング]」が [!UICONTROL 名前の入力を開始] フィールドに入力します。
1. 選択 [!UICONTROL マーケティングPortfolio] フィルタリング対象の同じ名前のポートフォリオがあるとします。 単に type ahead 機能を使用して目的のポートフォリオを見つけない場合。
1. クリック **[!UICONTROL フィルターを保存]**.

## アクティビティ 2 — 今月のクローズを自分が所有するプロジェクト

このビデオでは、 [!UICONTROL レガシーフィルター] エクスペリエンス。 多くのプロジェクトに目を向けている場合は、このフィルターを使用して、間もなく閉じる予定のプロジェクトを拡大できます。

詳細な手順の説明がページの後半にあります。

>[!VIDEO](https://video.tv.adobe.com/v/336807/?quality=12&learn=on)

### アクティビティ 2 に対する回答

![新しいフィルターを作成する画面の画像](assets/basic-filter-activity-updated-6-15-21.png)

1. [!UICONTROL メインメニュー]から[!UICONTROL プロジェクト]エリアに移動します。プロジェクトのリストが表示されます。
1. 次をクリック： **[!UICONTROL フィルター]** メニューと選択 [!UICONTROL レガシーフィルター].
1. 選択 **[!UICONTROL 新しいフィルター]**.
1. フィルターに「今月末に自分が所有するプロジェクト」という名前を付けます。
1. 「**[!UICONTROL フィルタールールを追加]**」をクリックします。
1. Adobe Analytics の [!UICONTROL フィールド名の入力を開始] 「所有者」と入力します。 それから、「[!UICONTROL プロジェクト]」フィールドソースの下にある「[!UICONTROL 所有者 ID]」を選択します。
1. 「[!UICONTROL 次と等しい]」演算子はそのままにしておきます。
1. 「$$」と入力して、 [!UICONTROL 名前の入力を開始] フィールドに入力します。
1. 「[!UICONTROL $$USER.ID]」を選択します。これは、ログイン中のユーザーに対するワイルドカードです。
1. もう一度「[!UICONTROL フィルタールールを追加]」をクリックします。
1. Adobe Analytics の [!UICONTROL フィールド名の入力を開始] フィールドに、「完了」と入力します。 それから、「プロジェクト」フィールドソースの下にある「[!UICONTROL 完了]」を選択します。
1. 「[!UICONTROL 次と等しい]」演算子はそのままにしておきます。
1. 「False」を選択します。
1. もう一度「[!UICONTROL フィルタールールを追加]」をクリックします。
1. Adobe Analytics の [!UICONTROL フィールド名の入力を開始] 「計画済み」フィールドタイプを選択し、「 [!UICONTROL 計画完了日] の下に [!UICONTROL プロジェクト] フィールドのソース。
1. 「[!UICONTROL 次と等しい]」演算子を「[!UICONTROL 今月]」に変更します。
1. クリック **[!UICONTROL フィルターを保存]**.
