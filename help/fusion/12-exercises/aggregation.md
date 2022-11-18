---
title: 集計
description: 複数の情報バンドルを 1 つの値に集計する方法を説明します。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11047
thumbnail: KT11047.png
exl-id: 4626b623-8b05-41be-9cfc-917e28222855
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# 集計

複数の情報バンドルを 1 つの値に集計する方法を説明します。

## 演習の概要

前の演習で作成した「反復の概要」シナリオを使用して、プロジェクト内の各作業タスクに関する計画時間を集計し、その情報を記載した電子メールを自分自身に送信します。

![集約画像 1](../12-exercises/assets/aggregation-walkthrough-1.png)

## 従う手順

**フィルターを追加し、計画時間を SUM します。**

1. 前の練習で作成した「反復の概要」シナリオのクローンを作成し、「集計の概要」という名前を付けます。
1. [ プロジェクトのタスクの読み込み ] モジュールと [ タスク数をカウント ] モジュールの間にフィルタを追加します。 フィルターに「作業中のタスクのみ」という名前を付けます。
1. 条件を「子の数」に設定します。 [数値演算子：次と等しい] 0.

   ![集約画像 2](../12-exercises/assets/aggregation-walkthrough-2.png)

1. Random Math モジュールの後に、Numeric Aggregator ツールモジュールを追加します。
1. ソースモジュールを「プロジェクトのタスクを読み取り」に設定します。
1. Aggregate 関数を SUM に設定します。
1. [ プロジェクトのタスクの読み込み ] モジュールの [ 作業 ] フィールドに値を設定します。
1. このモジュールの名前を&quot;SUM of all task pln hours&quot;に変更します。

   ![集約画像 3](../12-exercises/assets/aggregation-walkthrough-3.png)

   **集計が反復を終了することを示すシャドウが表示されます。**

   ![集約画像 4](../12-exercises/assets/aggregation-walkthrough-4.png)

   **時間を集計して電子メールを送信します。**

1. 数値集約の後に、電子メールアプリから電子メールを送信モジュールを追加します。
1. 自分にメールを送信します。
1. 件名は「Project details」です。
1. 「コンテンツ」フィールドに、「 [プロジェクト名] その数は [結果] 予定時間」 「[プロジェクト名]」は、「レコードの読み取り」モジュールおよび「[結果]」は、集約モジュールから取得されます。

   ![集約画像 5](../12-exercises/assets/aggregation-walkthrough-5.png)

1. 保存して 1 回実行します。 インボックス内の電子メールを確認します。

繰り返し内では、個々のバンドルにアクセスできます。 ただし、この反復以外では、 E メールを送信モジュールでは、集計フィールドのみにアクセスできます。
