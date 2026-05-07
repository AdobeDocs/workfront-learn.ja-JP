---
title: フィルターの演習
description: モジュール間のフィルターを使用して、特定のタイプのバンドルのみを通過させる方法について説明します。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11040
thumbnail: KT1101.png
recommendations: noDisplay,catalog
exl-id: d2cec1ea-7ff9-48ae-8bfb-0c767d346079
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:43:22.961Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 230
ht-degree: 100%

---

# フィルターの演習

モジュール間のフィルターを使用して、特定のタイプのバンドルのみを通過させる方法について説明します。

## 演習の概要

「基本マッピングを超える」シナリオの 2 つのモジュール間にフィルターを追加して、CSV ファイルでプロジェクトカラーが「赤」のプロジェクトのみを作成します。

![フィルター画像 1](../12-exercises/assets/filters-walkthrough-1.png)

## 手順

1. 「基本マッピングを超える」シナリオのクローンを作成し、「強力なフィルターの使用」という名前を付けます。

   **Workfront を作成プロジェクトモジュールの前にフィルターを追加して、赤いプロジェクトのみを作成できるようにします。**

   ![フィルター画像 2](../12-exercises/assets/filters-walkthrough-2.png)

1. フィルターを追加するには、モジュール間を結ぶ点線をクリックするか、レンチをクリックして「フィルターを設定」を選択します。
1. 「ラベル」フィールドを使用して、フィルターに「赤のプロジェクトのみ」という名前を付けます。
1. 「条件」フィールドで、「プロジェクトカラー」フィールド（CSV ファイルの列 3）をマッピングします。 次と等しい（大文字と小文字を区別しない）演算子を選択し、「赤」と入力します。
1. 「OK」をクリックします。

   ![フィルター画像 3](../12-exercises/assets/filters-walkthrough-3.png)

   **フィルターをテストし、結果を確認します。**

1. 「保存」をクリックしてシナリオを保存し、「1 回実行」をクリックします。
1. フィルターの実行インスペクターをクリックして、各バンドルがフィルターによってどのように検査され、Workfront を作成プロジェクトモジュールに移動するために成功したか失敗したかを確認します。

   ![フィルター画像 4](../12-exercises/assets/filters-walkthrough-4.png)

1. Workfront インスタンスで作成したプロジェクトを検索します。
