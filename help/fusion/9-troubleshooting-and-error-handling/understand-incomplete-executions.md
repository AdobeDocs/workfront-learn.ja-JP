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
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: ht
source-wordcount: '261'
ht-degree: 100%

---

# 不完全な実行について

不完全な実行は Workfront Fusion に保存でき、後で確認して解決できます。この優れた機能を活用する方法を説明します。

このビデオでは、以下について説明します。

* 不完全な実行とは
* 不完全な実行につながるエラーの処理方法

>[!VIDEO](https://video.tv.adobe.com/v/335307/?quality=12&learn=on&enablevpops=1)

## 不完全な実行につながるエラー

不完全な実行が保存される原因となるエラーには、いくつかのカテゴリがあります。

受信するエラータイプは、接続先の API によって異なります。エラーは、不完全なデータまたは誤ったデータから発生する検証エラーである可能性があります。ほとんどの場合、モジュールを通過するすべてのデータを正常に処理するために期待される項目が欠落していることが原因です。または、一時的または長期的な接続障害（メールまたはリモート FTP サーバーへの接続中など）が原因で、最終的な宛先が使用できないのでエラーが発生する可能性があります。

シナリオの最初のモジュールでエラーが発生した場合、実行は直ちに停止し、不完全な実行は保存されません。

他のモジュールでエラーが発生し、エラーハンドラールートが添付されていない場合は、次のようになります。

* エラータイプが ConnectionError、RateLimitError、OutOfSpaceError、ModuleTimeoutError の場合、自動再試行付きの不完全な実行レコードが保存されます。
* エラータイプが DataError、InvalidConfigurationError、InvalidAccessTokenError、UnexpectedError、MaxFileSizeExceededError、MaxResultsExceededError の場合、自動再試行なしの不完全な実行レコードが保存されます。
* エラータイプが上記以外の場合、実行は失敗します。

## 詳細情報 以下をお勧めします。

[Workfront Fusion ドキュメント](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
