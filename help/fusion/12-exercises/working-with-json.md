---
title: JSON の操作の演習
description: シナリオ内で JSON を作成および解析して、デザインのニーズに対応する方法を説明します。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11056
thumbnail: KT11056.png
recommendations: noDisplay,noCatalog
exl-id: 72d5159e-72e5-4202-90de-753b3d7626de
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 100%

---

# JSON の操作の演習

シナリオ内で JSON を作成および解析して、デザインのニーズに対応する方法を説明します。

## 演習の概要

この演習の目的は、シナリオに送信された情報を JSON 形式で利用し、シナリオ全体でマッピングできるフィールドとアイテムに解析する方法を概念的に示すことです。その後、マッピングされた配列から情報を取得するか、情報を JSON に集計して、JSON を受信入力として期待する別のシステムに送信できます。

![JSON の操作画像 1](../12-exercises/assets/working-with-json-walkthrough-1.png)

## 手順

**データ構造を作成し、JSON を解析します。**

1. 新しいシナリオを作成し、「JSON ドーナツデータの操作」という名前を付けます。
1. トリガーモジュールには、「変数を設定」モジュールを使用します。
1. 変数名に「ドーナツデータ」と入力します。
1. 変数値には、テストドライブの Fusion Exercise Files フォルダーにある「_Donut Data - Sample JSON.rtf」ドキュメントの内容をコピーして貼り付けます。

   ![JSON の操作画像 2](../12-exercises/assets/working-with-json-walkthrough-2.png)

1. このモジュールの名前を「別のコネクタからの JSON」に変更します。
1. 「JSON を解析」モジュールを追加します。
1. 「データ構造」フィールドの「追加」をクリックします。
1. 「ジェネレーター」を選択し、「サンプルデータ」フィールドにコピーした「ドーナツデータ — サンプル JSON データ」を貼り付けます。

   ![JSON の操作画像 3](../12-exercises/assets/working-with-json-walkthrough-3.png)

1. 「保存」をクリックし、データ構造に「ドーナツデータ」という名前を付けます。次に「保存」をクリックします。
1. 「変数を設定」モジュールのドーナツデータを「JSON 文字列」フィールドにマッピングします。

   ![JSON の操作画像 4](../12-exercises/assets/working-with-json-walkthrough-4.png)

1. シナリオを保存し、「1 回実行」をクリックして出力を表示します。

   **「JSON を解析」モジュールの出力は次のようになります。**

   ![JSON の操作画像 5](../12-exercises/assets/working-with-json-walkthrough-5.png)

   **特定の配列変数にマッピングします。**

1. 「JSON を解析」モジュールの後にルーターを追加します。
1. 上部のパスに「変数を設定」モジュールを追加します。
1. 「変数名」に「ドーナツ別の生地の種類」と入力します。
1. 変数値には、map 関数を使用して、生地の配列から記事の種類を取得します。

   ![JSON の操作画像 6](../12-exercises/assets/working-with-json-walkthrough-6.png)

1. 「OK」をクリックし、「1 回実行」をクリックします。
1. 実行インスペクターを開き、3 つの各操作の出力バンドルを確認し、それぞれの生地のタイプを表示します。

   ![JSON の操作画像 7](../12-exercises/assets/working-with-json-walkthrough-7.png)

   **シナリオデータを JSON に集計します。**

1. 下のルーティングパスに「JSON に集計」モジュールを追加します。
1. ソースモジュールには、イテレータ（「JSON 解析」モジュール）を選択します。
1. データ構造には、任意のデータ構造を作成するか選択します。この例では、ドーナツデータを使用します。
1. 次に示すように、この例のフィールドを直接マッピングします。
1. 生地とトッピングを取得すると、これらは配列であることがわかります。そのため、「アイテムを追加」をクリックして、マッピングする必要があります。

   ![JSON の操作画像 8](../12-exercises/assets/working-with-json-walkthrough-8.png)

1. シナリオを保存し、「1 回実行」をクリックします。

「JSON に集計」モジュールの実行インスペクターを確認すると、3 つのバンドルが 1 つの JSON 文字列に集計できたことがわかります。その後、この文字列を JSON を待ち受ける他のシステムに送信できます。

![JSON の操作画像 9](../12-exercises/assets/working-with-json-walkthrough-9.png)
