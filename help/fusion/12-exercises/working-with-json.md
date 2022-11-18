---
title: JSON の操作
description: シナリオ内で JSON を作成および解析して、デザインのニーズに対応する方法を説明します。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11056
thumbnail: KT11056.png
exl-id: 72d5159e-72e5-4202-90de-753b3d7626de
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# JSON の操作

シナリオ内で JSON を作成および解析して、デザインのニーズに対応する方法を説明します。

## 演習の概要

この演習の目的は、概念的に、シナリオに送信された情報を JSON 形式で利用し、シナリオ全体でマッピングできるフィールドと項目に解析する方法を示すことです。 次に、マッピングされた配列から情報を取得するか、情報を JSON に集計して、JSON を受信入力として期待する別のシステムに送信できます。

![JSON 画像 1 の操作](../12-exercises/assets/working-with-json-walkthrough-1.png)

## 従う手順

**データ構造を作成し、JSON を解析します。**

1. 新しいシナリオを作成し、「JSON ドーナツデータの使用」という名前を付けます。
1. トリガーモジュールには、変数設定モジュールを使用します。
1. 変数名に「ドーナツデータ」と入力します。
1. Variable 値に対して、テストドライブの Fusion Exercise Files フォルダにある「_Donut Data - Sample JSON.rtf」ドキュメントの内容をコピーして貼り付けます。

   ![JSON 画像 2 の操作](../12-exercises/assets/working-with-json-walkthrough-2.png)

1. このモジュールの名前を「別のコネクタからの JSON」に変更します。
1. 解析 JSON モジュールを追加します。
1. 「データ構造」フィールドの「追加」をクリックします。
1. 「ジェネレーター」を選択し、「サンプルデータ」フィールドにコピーした「ドーナツデータ — サンプル JSON データ」を貼り付けます。

   ![JSON 画像の使用 3](../12-exercises/assets/working-with-json-walkthrough-3.png)

1. 「保存」をクリックし、データ構造に「ドーナツデータ」という名前を付けます。 次に、「保存」をクリックします。
1. 「変数を設定」モジュールのドーナツデータを「 JSON 文字列」フィールドにマッピングします。

   ![JSON 画像の操作 4](../12-exercises/assets/working-with-json-walkthrough-4.png)

1. シナリオを保存し、「1 回実行」をクリックして出力を表示します。

   **解析 JSON モジュールの出力は次のようになります。**

   ![JSON 画像の操作 5](../12-exercises/assets/working-with-json-walkthrough-5.png)

   **特定の配列変数にマッピングします。**

1. Parse JSON モジュールの後にルータを追加します。
1. 上部のパスに変数を設定モジュールを追加します。
1. 「変数名」に「ドーナツタイプ別」と入力します。
1. Variable 値には、 map 関数を使用して、バッター配列からバッター型を取得します。

   ![JSON 画像 6 の操作](../12-exercises/assets/working-with-json-walkthrough-6.png)

1. 「OK」をクリックし、「1 回実行」をクリックします。
1. 実行インスペクターを開き、3 つの各操作の出力バンドルを確認し、それぞれのバッタータイプを表示します。

   ![JSON 画像の操作 7](../12-exercises/assets/working-with-json-walkthrough-7.png)

   **シナリオデータを JSON に集計します。**

1. 下のルーティングパスに、「Aggregate to JSON」モジュールを追加します。
1. ソースモジュールの場合は、イテレータ（「解析 JSON」モジュール）を選択します。
1. データ構造の場合は、任意のデータ構造を作成するか選択します。 この例では、ドーナツデータを使用します。
1. 次に示すように、この例のフィールドを直接マッピングします。
1. バッターとトッピングを取得したら、配列であることに注意してください。「項目を追加」をクリックして、マッピングする必要があります。

   ![JSON 画像の操作 8](../12-exercises/assets/working-with-json-walkthrough-8.png)

1. シナリオを保存し、「1 回実行」をクリックします。

「 JSON に集計」モジュールの実行インスペクターを見て、3 つのバンドルを 1 つの JSON 文字列に集計する方法を確認します。 その後、この文字列を JSON を想定する他のシステムに送信できます。

![JSON 画像 9 の操作](../12-exercises/assets/working-with-json-walkthrough-9.png)
