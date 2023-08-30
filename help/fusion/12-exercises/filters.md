---
title: フィルター
description: モジュール間のフィルターを使用して、特定のタイプのバンドルのみを通過させる方法について説明します。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11040
thumbnail: KT1101.png
exl-id: d2cec1ea-7ff9-48ae-8bfb-0c767d346079
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '223'
ht-degree: 100%

---

# フィルター

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
1. 「条件」フィールドで、「プロジェクトカラー」フィールド（CSV ファイルの列 3）をマッピングします。次と等しい（大文字と小文字を区別しない）演算子を選択し、「赤」と入力します。
1. 「OK」をクリックします。

   ![フィルター画像 3](../12-exercises/assets/filters-walkthrough-3.png)

   **フィルターをテストし、結果を確認します。**

1. 「保存」をクリックしてシナリオを保存し、「1 回実行」をクリックします。
1. フィルターの実行インスペクターをクリックして、各バンドルがフィルターによってどのように検査され、Workfront を作成プロジェクトモジュールに移動するために成功したか失敗したかを確認します。

   ![フィルター画像 4](../12-exercises/assets/filters-walkthrough-4.png)

1. Workfront インスタンスで作成したプロジェクトを検索します。
