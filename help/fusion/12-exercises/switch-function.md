---
title: 切り替え機能
description: スイッチ機能を使用したスイッチ機能の使用方法を説明します。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11051
thumbnail: KT1101.png
exl-id: 3142fae2-5210-4f63-9d2c-66dec58867fa
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# 切り替え機能

スイッチ機能を使用したスイッチ機能の使用方法を説明します。

## 演習の概要

単純なデータ変更の場合は、 Switch 関数を使用して、モジュールフィールド内の値を別の値に変換します。 この練習では、2 文字のキーを、プロジェクトの進行状況ステータスの実際の名前に変更し、E メールで送信します。

![スイッチ機能画像 1](../12-exercises/assets/switch-function-walkthrough-1.png)

## 従う手順

1. 「ルーティングパス間での変数の共有」というシナリオを複製します。
1. 新しいシナリオに「Sharing variables between routing paths - Switch」という名前を付けます。
1. 「トリガー」モジュールをクリックし、「出力」セクションに「進捗状況ステータス」を追加します。
1. 「 E メールを送信」モジュールで、「コンテンツ」フィールドに進捗状況ステータスを追加します。

   + 検索モジュールから取得した値の上にマッピングするだけの場合、進行状況ステータスを示す 2 文字のコードが表示されます。
   + 可能な各進捗状況ステータスのフルネームのコードを「切り替え」るには、「一般関数」タブの「切り替え」機能を使用します。

1. switch 関数は、Progress Status の値または式をキーとして使用し、そのキーに基づいて出力値を返します。

   + キー値は、2 番目の位置（「遅延」）で定義された対応する出力と共に、進捗状況ステータス (「LT」) の後の最初の位置で定義されます。
   + 次のキー値は、第 3 位置で定義され、対応する出力は第 4 位置等で必要な数のキーに対して定義される。

      ![スイッチ機能画像 2](../12-exercises/assets/switch-function-walkthrough-2.png)
