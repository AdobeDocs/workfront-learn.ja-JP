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
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: ht
source-wordcount: '318'
ht-degree: 100%

---

# エラー処理ディレクティブについて

このビデオでは、次のことを学習します。

* 実行を続行できる 3 つのエラーハンドラーディレクティブ
* 実行を停止する 2 つのエラーハンドラーディレクティブ

>[!VIDEO](https://video.tv.adobe.com/v/3418138/?quality=12&learn=on&enablevpops&captions=jpn)

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
