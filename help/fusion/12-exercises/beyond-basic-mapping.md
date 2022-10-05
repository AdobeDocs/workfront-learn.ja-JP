---
title: 基本マッピングを超える
description: マッピングパネルの数式を使用して、モジュールに送信されるフィールドを操作または変換する方法を説明します。
feature: Workfront Fusion
role: User
level: Beginner
kt: 11039
thumbnail: KT11039.png
source-git-commit: c348222464180e994e7b414d1b84e07f58b6b2ae
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---


# 基本マッピングを超える

マッピングパネルの数式を使用して、モジュールに送信されるフィールドを操作または変換する方法を説明します。

## 演習の概要

[ マッピング ] パネルの式を使用して、[ 基本マッピングを超える ] の演習から、プロジェクト名、計画開始日、優先度を変更します。

![基本マッピング画像 1 を超えています](../12-exercises/assets/beyond-basic-mapping-walkthrough-1.png)

## 従う手順

**初期シナリオデザインシナリオのクローンを作成します。**

1. 次に示すように、シナリオセクションの最初のシナリオデザインの右側にある「クローン」オプションを選択します。 「Beyond basic mapping」という名前を付けます。

   ![Beyond Basic Mapping Image 2](../12-exercises/assets/beyond-basic-mapping-walkthrough-2.png)

   **次に、Workfrontプロジェクト作成モジュールのマッピングパネルを使用して、プロジェクト名、計画開始日、優先度の各フィールドを設定します。**

1. 「 Workfrontプロジェクトを作成」モジュールをクリックして、設定を編集します。 マッピングパネルを使用して、「名前」フィールドを「[マイプロジェクト名] 作成者 [スポンサー].&quot;

   + この [マイプロジェクト名] は、「 CSV を解析」モジュールの列 1 で、 [スポンサー] は列 6 です。 「by」という単語は、2 つの間に入力するだけです。

1. 次に、「 Beyond basic mapping walkthrough video 」の説明に従って、「 Planned Start Date 」に移動し、 addDays 数式を使用して 15 日を「 」フィールドに追加します。
1. 「優先度」フィールドを見つけ、フィールドの右上にある「マップ」ボタンを切り替えます。 選択リストメニューが数値に変わります。 CSV ファイルの信頼性評価が 100 未満の場合は、プロジェクトに高 (4) 優先度というラベルを付ける if 文を作成します。それ以外の場合は、Normal(2) を作成します。

   + 信頼性評価は列 4 です。

   **この時点で、マッピングパネルは次のようになります。**

   ![Beyond Basic Mapping Image 3](../12-exercises/assets/beyond-basic-mapping-walkthrough-3.png)

1. 「 OK 」をクリックし、「実行」を 1 回クリックします。
1. Workfrontインスタンスでプロジェクトを見つけ、すべてが正しくマッピングされていることを確認します。
1. シナリオを保存します。
