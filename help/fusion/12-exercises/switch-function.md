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
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:41:24.173Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 240
ht-degree: 100%

---

# switch 関数の演習

スイッチ関数を使用した切り替え機能の使用方法を説明します。

## 演習の概要

単純なデータ変更の場合は、スイッチ関数を使用して、モジュールフィールド内の値を別の値に変換します。 この演習では、2 文字のキーをプロジェクトの進捗ステータスの実際の名前に変更し、メールで送信します。

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
