---
title: 不完全な実行を理解する
description: 実行が不完全な部分と、で実行が不完全になるエラーを処理する方法について説明します。 [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: Jira ticket
exl-id: 3b7bf669-4736-4ba5-bcec-0d3fe0b2ce74
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# 不完全な実行を理解する

不完全な実行は、Workfront Fusion に保存され、後で確認および解決できます。 この素晴らしい機能を活用する方法を学びます。

このビデオでは、次のことを学習します。

* 実行が不完全な部分は何か
* 実行が不完全になるエラーの処理方法

>[!VIDEO](https://video.tv.adobe.com/v/335307/?quality=12)

## 実行が不完全な原因となるエラー

実行が不完全な状態で保存される原因となるエラーには、いくつかのカテゴリがあります。

受け取るエラータイプは、接続先の API によって異なります。 このエラーは、不完全なデータまたは誤ったデータに起因する検証エラーの可能性があります。これは、モジュールを通過するすべてのデータを正常に処理するために予期される項目が欠落しているためです。 または、一時的または長期的な接続障害（電子メールやリモート FTP サーバーへの接続中など）が原因で、最終的な宛先が使用できなくなったことがエラーの原因となる場合があります。

シナリオの最初のモジュールでエラーが発生した場合、実行は直ちに停止し、不完全な実行は保存されません。

他のモジュールでエラーが発生し、エラーハンドラールートが添付されていない場合は、次のようになります。

* エラーの種類が ConnectionError、RateLimitError、OutOfSpaceError、または ModuleTimeoutError の場合、不完全な実行レコードが自動再試行付きで保存されます。
* エラーの種類が DataError、InvalidConfigurationError、InvalidAccessTokenError、UnexpectedError、MaxFileSizeExceededError または MaxResultsExceededError の場合、不完全な実行レコードが自動再試行なしで保存されます。
* エラータイプが上記以外の場合、実行は失敗します。

## 詳細情報 以下をお勧めします。

[Workfront Fusion ドキュメント](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
