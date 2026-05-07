---
title: 不完全な実行について
description: ' [!DNL Adobe Workfront Fusion] での不完全な実行と、不完全な実行につながるエラーの処理方法を説明します。'
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9066
exl-id: 3b7bf669-4736-4ba5-bcec-0d3fe0b2ce74
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
autotag-review: '2026-05-06T16:07:51.152Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 280
ht-degree: 100%

---

# 不完全な実行について

不完全な実行は Workfront Fusion に保存でき、後で確認して解決できます。 この優れた機能を活用する方法を説明します。

このビデオでは、以下について説明します。

* 不完全な実行とは
* 不完全な実行につながるエラーの処理方法

>[!VIDEO](https://video.tv.adobe.com/v/3418151/?captions=jpn&quality=12&learn=on&enablevpops=1)

## 不完全な実行につながるエラー

不完全な実行が保存される原因となるエラーには、いくつかのカテゴリがあります。

受信するエラータイプは、接続先の API によって異なります。 エラーは、不完全なデータまたは誤ったデータから発生する検証エラーである可能性があります。ほとんどの場合、モジュールを通過するすべてのデータを正常に処理するために期待される項目が欠落していることが原因です。 または、一時的または長期的な接続障害（メールまたはリモート FTP サーバーへの接続中など）が原因で、最終的な宛先が使用できないのでエラーが発生する可能性があります。

シナリオの最初のモジュールでエラーが発生した場合、実行は直ちに停止し、不完全な実行は保存されません。

他のモジュールでエラーが発生し、エラーハンドラールートが添付されていない場合は、次のようになります。

* エラータイプが ConnectionError、RateLimitError、OutOfSpaceError、ModuleTimeoutError の場合、自動再試行付きの不完全な実行レコードが保存されます。
* エラータイプが DataError、InvalidConfigurationError、InvalidAccessTokenError、UnexpectedError、MaxFileSizeExceededError、MaxResultsExceededError の場合、自動再試行なしの不完全な実行レコードが保存されます。
* エラータイプが上記以外の場合、実行は失敗します。

## 詳細情報 以下をお勧めします。

[Workfront Fusion のドキュメント](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
