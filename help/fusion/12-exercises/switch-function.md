---
title: switch 関数の演習
description: スイッチ関数を使用した切り替え機能の使用方法を説明します。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11051
thumbnail: KT1101.png
recommendations: noDisplay,catalog
exl-id: 3142fae2-5210-4f63-9d2c-66dec58867fa
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: ht
source-wordcount: '238'
ht-degree: 100%

---

# switch 関数の演習

スイッチ関数を使用した切り替え機能の使用方法を説明します。

## 演習の概要

単純なデータ変更の場合は、スイッチ関数を使用して、モジュールフィールド内の値を別の値に変換します。この演習では、2 文字のキーをプロジェクトの進捗ステータスの実際の名前に変更し、メールで送信します。

![スイッチ関数の画像 1](../12-exercises/assets/switch-function-walkthrough-1.png)

## 手順

1. 「ルーティングパス間での変数の共有」というシナリオを複製します。
1. 新しいシナリオに「ルーティングパス間での変数の共有（スイッチ）」という名前を付けます。
1. トリガーモジュールをクリックし、「出力」セクションに「進捗ステータス」を追加します。
1. 「メールを送信」モジュールで、「コンテンツ」フィールドに「進捗ステータス」を追加します。

   + 「検索」モジュールから取得した値の上にマッピングするだけの場合、進捗ステータスを示す 2 文字のコードが表示されます。
   + コードを各進捗ステータスのフルネームに「切り替える」には、「一般関数」タブの「スイッチ」関数を使用します。

1. スイッチ関数は、進捗ステータスの値または式をキーとして使用し、そのキーに基づいて出力値を返します。

   + キー値は進捗ステータス（LT）の後の最初の位置で定義され、対応する出力（遅延）は 2 番目の位置で定義されます。
   + 次のキー値は 3 番目の位置で定義され、それに対応する出力は 4 番目の位置で定義されます。このようにして、必要な数のキーに対して定義されます。

     ![スイッチ関数の画像 2](../12-exercises/assets/switch-function-walkthrough-2.png)
