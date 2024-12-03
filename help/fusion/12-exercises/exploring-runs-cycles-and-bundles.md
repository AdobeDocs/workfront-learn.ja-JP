---
title: 実行、サイクル、バンドルの探索の演習
description: シナリオの実行履歴を使用して、実行、サイクル、バンドルの動作方法について説明します。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11050
thumbnail: KT1101.png
recommendations: noDisplay,catalog
exl-id: f04c84b1-2a3c-418b-9db3-baa74cf364f3
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 100%

---

# 実行、サイクル、バンドルの探索の演習

シナリオの実行履歴を使用して、実行、サイクル、バンドルの動作方法について説明します。

## 演習の概要

実行とサイクルを使用して調べる様々なシナリオ設定を実習します。

![実行、サイクル、バンドルの調査の画像 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)

## 手順

1. 「ルーティングパス間での変数の共有」というシナリオを複製します。新しいシナリオに「ルーティングパス間での変数の共有（サイクルテスト）」という名前を付けます。
1. このテストには必要ないので、メールを送信モジュールを削除します。

   **実行ごとに 3 サイクルを処理するようにシナリオを設定します。各サイクルで 5 つのプロジェクトを処理します。**

1. トリガーモジュールをクリックし、「最大」フィールドを 5 に変更して、各サイクルで 5 つのプロジェクトのみが処理されるようにします。
1. 検索条件で、検索を 1 つのプロジェクトに制限する 2 番目のフィルターを削除します。
1. 「OK」をクリックします。

1. Fusion ツールバーで、シナリオ設定を開き、「最大サイクル数」フィールドを 1 から 3 に変更します。
1. 「OK」をクリックします。

   ![実行、サイクル、バンドルの調査の画像 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)


   **シナリオを毎分実行するようにスケジュールします。**

1. トリガーモジュールの横にある時計アイコンをクリックし、「分」フィールドを 1 分に変更します。

   ![実行、サイクル、バンドルの調査の画像 2](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-2.png)

1. 次に、「1 回実行」ボタンの下にある「スケジュール」切替スイッチをオンに切り替えます。 シナリオを保存します。

   ![実行、サイクル、バンドルの調査の画像 3](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-3.png)

1. シナリオの実行履歴に移動し、次の 1 分以内に新しい履歴レコードが表示されるのを確認します。ページを更新する必要がある場合があります。

   ![実行、サイクル、バンドルの調査の画像 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-4.png)

1. 実行の「詳細」ボタンをクリックします。Workfront Fusion トレーニングの実行履歴部分で行ったのと同様に、右側のパネルのシンプルログをクリックします。
1. 処理された操作の記録は、サイクルに分割されます。

   ![実行、サイクル、バンドルの調査の画像 5](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-5.png)

1. ウィンドウの右上にあるドロップダウンメニューを使用すると、毎回実行するように設定した 3 つのサイクルのいずれかを選択できます。

   ![実行、サイクル、バンドルの調査の画像 6](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-6.png)
