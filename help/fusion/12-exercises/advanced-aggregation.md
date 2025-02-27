---
title: 詳細な集計の演習
description: Web サービスを呼び出して複数の国に関する詳細を返し、サブ地域ごとにグループ化された母集団を特定します。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11048
thumbnail: KT11048.png
recommendations: noDisplay,catalog
exl-id: 5364befa-491d-4b75-b1f0-10244f70ad7c
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: ht
source-wordcount: '0'
ht-degree: 100%

---

# 詳細な集計の演習

集計時のグループ化の使用方法について説明します。

## 演習の概要

Web サービスを呼び出して複数の国に関する詳細を返し、サブ地域ごとにグループ化されたすべての国の総母集団を特定します。

![詳細な集計の画像 1](../12-exercises/assets/advanced-aggregation-walkthrough-1.png)

## 手順

**国の詳細を取得します。**

![詳細な集計の画像 2](../12-exercises/assets/advanced-aggregation-walkthrough-2.png)

1. 新しいシナリオを作成し、「詳細な集計」という名前を付けます。
1. トリガーモジュールを HTTP - リクエストを行うモジュールに設定します。
1. この URL `https://restcountries.com/v2/lang/es` を使用すると、スペイン語圏のすべての国のリストが表示されます。
1. メソッドは Get のままにします。
1. 「応答を解析」チェックボックスをクリックします。
1. このモジュールの名前を「国を取得」に変更します。
1. 「保存」をクリックし、「1 回実行」をクリックします。

   **出力は 1 つのバンドルですが、スペイン語圏の国ごとに 1 つずつ、24 のコレクションを含む配列になっています。**

   ![詳細な集計の画像 3](../12-exercises/assets/advanced-aggregation-walkthrough-3.png)

   **国ごとにサブ地域情報を収集する必要があるので、追加の HTTP リクエストを行う必要があります。**

1. サブ地域情報を取得する別のリクエストを追加します。最初の国のみが返されますが、今は問題ありません。別の HTTP リクエストを行うモジュールを追加し、URL `https://restcountries.com/v2/name/{country name}` を使用します。
1. 最初の国名を取得するには、マッピングパネルに移動し、「データ」をクリックしてから、配列内の「名前」をクリックします。データフィールドの [1] では、配列の最初の項目を返します。

   + 数字をクリックし、必要に応じてインデックスを変更しますが、この場合は最初の項目だけが必要です。

![詳細な集計の画像 4](../12-exercises/assets/advanced-aggregation-walkthrough-4.png)

1. マッピングパネルで「応答を解析」をオンにして、「OK」をクリックします。
1. この名前を「国の詳細を取得」に変更します。
1. 「保存」、「1 回実行」の順にクリックします。

   + 出力されるのは、1 つの国の情報です。

1. その他の国を取得するには、配列を繰り返し処理する必要があります。物のリストを受け取り、リストの各項目のバンドルを出力するイテレータを追加します。

   **イテレータとアグリゲータを追加します。**

1. HTTP モジュール間を右クリックし、イテレータフローコントロールモジュールを追加します。
1. 「配列」フィールドで、国を取得モジュールから「データ」を選択します。

   ![詳細な集計の画像 5](../12-exercises/assets/advanced-aggregation-walkthrough-5.png)

1. 国の詳細を取得モジュールで URL フィールドを更新して、国を取得モジュールではなくイテレータから名前フィールドを取得します。

   ![詳細な集計の画像 6](../12-exercises/assets/advanced-aggregation-walkthrough-6.png)

1. 「国の詳細を取得」の後に数値アグリゲータを追加し、母集団をグループ化して合計します。
1. ソースモジュールは、イテレータモジュールです。
1. 集計関数は SUM です。
1. 値は、国の詳細を取得モジュールの [data:population] です。
1. 下部にある「詳細設定を表示」オプションをクリックし、国の詳細を取得モジュールから [data:subregion] でグループ化します。

   ![詳細な集計の画像 7](../12-exercises/assets/advanced-aggregation-walkthrough-7.png)

   **テキスト集約関数で終了し、数値アグリゲータ内でグループ化したものを集計します。**

1. テキストアグリゲータを最後に追加します。
1. ソースモジュールは、数値アグリゲータです。
1. テキストエリアに、「[キー] の総母集団は[結果]です」と挿入します。

   ![詳細な集計の画像 8](../12-exercises/assets/advanced-aggregation-walkthrough-8.png)

1. 保存して 1 回実行します。

   + 最終モジュールからの出力をレビューします。
