---
title: フィルター
description: モジュール間のフィルターを使用して、特定の種類のバンドルのみを許可する方法を説明します。
feature: Workfront Fusion
role: User
level: Beginner
kt: 11040
thumbnail: KT1101.png
source-git-commit: f367e016498d5c1814cab79e19e6e9001db2851f
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---


# フィルター

モジュール間のフィルターを使用して、特定の種類のバンドルのみを許可する方法を説明します。

## 演習の概要

Beyond basic mapping シナリオで 2 つのモジュール間にフィルターを追加して、CSV ファイル内に「赤」のプロジェクト色を持つプロジェクトのみを作成します。

![画像 1 をフィルター](../12-exercises/assets/filters-walkthrough-1.png)

## 従う手順

1. 「基本的なマッピングを超えた」シナリオのクローンを作成し、「強力なフィルターの使用」という名前を付けます。

   **赤いプロジェクトのみを作成できるように、Workfrontプロジェクト作成モジュールの前にフィルターを追加します。**

   ![画像 2 をフィルター](../12-exercises/assets/filters-walkthrough-2.png)

1. フィルターを追加するには、モジュール間を結ぶ点線をクリックするか、レンチをクリックし、「フィルターを設定する」を選択します。
1. 「ラベル」フィールドを使用して、フィルターに「Only Red Projects」という名前を付けます。
1. 「条件」フィールドで、「プロジェクトの色」フィールド（CSV ファイルの列 3）をマッピングします。 次と等しい（大文字と小文字を区別しない）演算子を選択し、「赤」と入力します。
1. 「OK」をクリックします。

   ![画像 3 をフィルター](../12-exercises/assets/filters-walkthrough-3.png)

   **フィルターをテストし、結果を確認します。**

1. 「保存」をクリックしてシナリオを保存し、「1 回実行」をクリックします。
1. フィルターの実行インスペクターをクリックして、各バンドルがフィルターによってどのように調べられ、Workfrontプロジェクトの作成モジュールに渡されたか、移動できなかったかを確認します。

   ![画像 4 をフィルター](../12-exercises/assets/filters-walkthrough-4.png)

1. Workfrontインスタンスで作成したプロジェクトを見つけます。
