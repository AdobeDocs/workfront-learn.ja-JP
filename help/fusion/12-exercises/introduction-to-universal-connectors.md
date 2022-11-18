---
title: ユニバーサルコネクタの概要
description: REST ユニバーサルコネクタの操作と、返されるデータの操作に関する理解を深めます。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11042
thumbnail: KT11042.png
exl-id: eb442c3e-26f3-44b7-9937-ed4eeba39fb1
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 0%

---

# ユニバーサルコネクタの概要

REST ユニバーサルコネクタの操作と、返されるデータの操作に関する理解を深めます。

## 演習の概要

スプレッドシートでポケモン文字を使用して、HTTP コネクタを介してポケモン API を呼び出し、その文字に関する詳細を収集して投稿します。

![ユニバーサルコネクタの概要画像 1](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-1.png)

## 従う手順

**Workfrontから CSV ファイルをダウンロードします。**

1. Workfrontの「Fusion Exersice Files」フォルダで、「_Fusion2020_Shipping Manifest.csv」を選択し、「ドキュメントの詳細」をクリックします。
1. URL アドレスから最初の ID 番号をコピーします。
1. Workfront Fusion で新しいシナリオを作成します。 これに、「Using universal connectors」という名前を付けます。
1. まず、Workfrontアプリからドキュメントをダウンロードモジュールを使用します。
1. Workfront接続を設定し、Workfront URL からコピーしたドキュメント ID を含めます。
1. このモジュールの名前を「Download shipping manifest」に変更します。

   ![ユニバーサルコネクタの概要画像 9](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-9.png)

   **発行マニフェストデータを解析します。**

1. 「 CSV を解析」を選択して、別のモジュールを追加します。
1. 11 列用に CSV を解析を設定します。 「 CSV にヘッダーを含む」ボックスをオンにします。 Comma delimiterType を選択し、「ドキュメントをダウンロード」モジュールのデータを「CSV」フィールドに入力します。

   ![ユニバーサルコネクタの概要画像 2](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-2.png)

1. このモジュールの名前を「Parse shipping manifest」に変更します。
1. シナリオを保存し、「 1 回実行」をクリックして、次の手順で CSV ファイルのデータを確認できます。

   **ユニバーサルコネクタを使用して Pokemon データを取得します。**

1. HTTP Make a Request モジュールを追加します。
1. URL フィールドで、 `https://pokeapi.co/api/v2/pokemon/[Character]`で、 [文字] は、「 CSV を解析」モジュールから列 3 にマッピングされます。
1. 「応答を解析」チェックボックスを選択します。
1. 「詳細設定を表示」を選択し、「すべての状態をエラーとして評価」の横にあるチェックボックスをオンにします。
1. 「OK」をクリックし、モジュール名を「Get Pokemon info」に変更します。

   **マッピングパネルは次のようになります。**

   ![ユニバーサルコネクタの概要画像 3](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-3.png)

   **この演習のこの部分では、CSV ファイルの行 1 のみを処理します。**

1. ポケモン情報を取得モジュールの前にフィルターを追加します。 「1 行目のみ」という名前を付けます。
1. ID 番号 1 のみを渡す条件を設定します。 ID 番号 1 が 1 行目に、ID フィールドが CSV ファイルの列 1 に入っています。

   ![ユニバーサルコネクタの概要画像 4](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-4.png)

1. シナリオを保存します。
1. 「1 回実行」をクリックし、HTTP Make リクエストモジュールで受け取るエラーメッセージを確認します。

   >[!IMPORTANT]
   >
   >入力データ URL フィールドでは、文字名が大文字であることに注意してください。 文字名を小文字にする必要があるので、この API 呼び出しは機能しません。

   ![ユニバーサルコネクタの概要画像 5](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-5.png)

1. 「 HTTP Make a request URL 」フィールドのマッピングパネルを使用して、 [文字] すべての小文字を **lower** 関数に置き換えます。

   ![ユニバーサルコネクタの概要（画像 6）](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-6.png)

   **複数変数を設定モジュールを使用して、API から情報をマッピングし直します。**

1. ポケモン情報を取得の後に、複数の変数を設定モジュールを追加します。 マップ名、高さ、重み、および能力。
1. 「アビリティー」フィールドは配列なので、必ず map 関数を使用して配列内の各アビリティーの名前にアクセスしてください。

   ![ユニバーサルコネクタの概要画像 7](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-7.png)

   **別のエラーを明らかにするには、フィルターを付けずにシナリオを実行します。**

1. CSV ファイル内のすべての行を処理するには、「行 1 のみ」という名前のフィルターを削除します。

   + フィルターアイコンをクリックして編集します。
   + フィルターラベルを削除します。
   + 条件を削除します。
   + 「OK」をクリックします。

1. シナリオを保存し、「1 回実行」をクリックします。
1. ポケモン情報の取得モジュールでエラーが発生しました。 スーパーヒーローキャラクターが Pokemon API に渡されているのがわかります。

   >[!NOTE]
   >
   >「Routers」のチュートリアルでは、スーパーヒーローを処理する別のパスを作成して、このエラーを解決する方法を確認します。

   ![ユニバーサルコネクタの概要画像 8](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-8.png)
