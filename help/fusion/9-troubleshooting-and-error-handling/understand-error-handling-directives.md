---
title: エラー処理ディレクティブについて
description: ' [!DNL Adobe Workfront Fusion] で、実行を続行できるエラーハンドラーディレクティブと、実行を停止するエラーハンドラーディレクティブについて説明します。'
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9064
exl-id: cb8d0880-73d2-4118-b800-a126f8509309
recommendations: noDisplay,catalog
doc-type: video
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
autotag-review: '2026-05-06T16:07:23.288Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 318
ht-degree: 100%

---

# エラー処理ディレクティブについて

このビデオでは、次のことを学習します。

* 実行を続行できる 3 つのエラーハンドラーディレクティブ
* 実行を停止する 2 つのエラーハンドラーディレクティブ

>[!VIDEO](https://video.tv.adobe.com/v/335305/?quality=12&learn=on&enablevpops=1)

## ディレクティブ - シナリオは続行します

### 再開

* エラーが発生したモジュールに代替出力が指定され、提供されます。
* 以降のモジュールが処理されます。
* シナリオの実行ステータスは「成功」とマークされます。

![再開ディレクティブの画像](assets/troubleshooting-and-error-handling-2.png)

### 一時停止

* シナリオの実行状態は、不完全な実行のキューに保存されます。このキューでは、エラーを手動で解決できます。 ただし、ここで言及する例外もいくつかあります。
* 後続のモジュールは処理されません。
* 未処理のバンドルがある場合、シナリオの実行は通常どおり続行されます。
* シナリオの実行ステータスは、「警告」とマークされます。

![一時停止ディレクティブの画像](assets/troubleshooting-and-error-handling-3.png)

### 無視

* エラーは無視され、後続のモジュールは処理されません。
* 未処理のバンドルがある場合、シナリオの実行は通常どおり続行されます。
* シナリオの実行ステータスは「成功」とマークされます。

![無視ディレクティブの画像](assets/troubleshooting-and-error-handling-4.png)

## ディレクティブ - シナリオが停止する

### ロールバック

* シナリオの実行は直ちに停止し、すべてのモジュールでロールバックフェーズが開始され、すべてのモジュールが初期状態に戻されます。
* 後続のモジュールは処理されません。
* いくつかのエラータイプがある場合、シナリオは、「シナリオ設定」で指定した「連続エラー数」の後で非アクティブ化されます。
* シナリオの実行ステータスは「エラー」とマークされます。

>[!NOTE]
>
>これは、モジュールにエラーハンドラールートが添付されておらず、「シナリオ」設定の「不完全な実行の保存を許可」設定がオフの場合のデフォルトの動作です。

![ロールバックディレクティブの画像](assets/troubleshooting-and-error-handling-5.png)

### コミット

* エラーは無視され、後続のモジュールは処理されません。
* 未処理のバンドルがある場合、シナリオの実行は通常どおり続行されます。
* シナリオの実行ステータスは「成功」とマークされます。

![コミットディレクティブの画像](assets/troubleshooting-and-error-handling-6.png)
