---
title: ルーティングパターンの演習
description: 他の API を実際に使用せずに、ルーティングとフォールバックルートの概念を強化します。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11044
thumbnail: KT11044.png
recommendations: noDisplay,catalog
exl-id: d8218115-5180-4e64-8ec1-d2d6afc88d23
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
autotag-review: '2026-05-06T16:42:16.496Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 361
ht-degree: 100%

---

# ルーティングパターンの演習

他の API を実際に使用せずに、ルーティングとフォールバックルートの概念を強化します。

## 演習の概要

変数設定モジュールを使用して、複数のパスを介して数値を送信し、ルーティング時にフィルターとフォールバックがどのように動作するかを確認します。

![ルーティングパターンの画像 1](../12-exercises/assets/routing-patterns-walkthrough-1.png)

## 手順

1. 新しいシナリオを作成し、「ルーティングパターンとフォールバック」と名付けます。
1. トリガーの場合、変数設定ツールモジュールを追加します。 変数名に「My Number」を入力し、変数の有効期間を 1 サイクルのままにして、変数フィールドを「75」に設定します。

   ![ルーティングパターンの画像 2](../12-exercises/assets/routing-patterns-walkthrough-2.png)

1. 別のモジュールを追加し、ルーターモジュールを選択します。 両方のパスに対して、Increment 機能ツールを選択し、それぞれに変更を加えることなく「OK」をクリックします。

   + 最初のパスに対して、フィルターを作成し、これに「100 未満」という名前を付け、[My Number] の条件を100 未満に設定します。

   + 2 番目のパスに対して、フィルターを作成し、これに「1000 未満」という名前を付け、[My Number] の条件を 1000 未満に設定します。 必ず、両方に数値演算子を使用します。

   ![ルーティングパターンの画像 3](../12-exercises/assets/routing-patterns-walkthrough-3.png)

   ![ルーティングパターンの画像 4](../12-exercises/assets/routing-patterns-walkthrough-4.png)

1. 「1 回実行」をクリックし、バンドルが「100 未満」のパスを渡すことを監視します。
1. 次に、変数モジュール設定フィールドを 950 に変更し、もう一度実行します。 2 つ目のパスの流れを監視します。
1. ルーターをクリックし、パスをもう 1 つ追加します。 Increment 関数ツールモジュールを追加します。 フィルターの場合は、「フォールバックルート」チェックボックスをクリックします。 そのパスを指す矢印が、フォールバック ルートを示すキャレットに変わることを確認します。

   ![ルーティングパターンの画像 5](../12-exercises/assets/routing-patterns-walkthrough-5.png)

1. 変数設定の数値を 9500 に変更し、1 回実行します。 この数値が 100 以上または 1000 未満であるため、バンドルはフォールバックルートをたどります。

Increment 関数ツールモジュールでもう 1 つのパスを追加しても、フィルターを設定しない場合に、もう一度「実行」をクリックすると何が起こるでしょうか。 バンドルは、4 番目のルートが追加された状態で、フォールバック ルートをたどるでしょうか。

+ いいえ。フィルターが設定されていないので、すべてのバンドルは常にフォールバックルートではなくこのパスをたどります。
