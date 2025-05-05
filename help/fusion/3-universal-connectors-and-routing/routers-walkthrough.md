---
title: ルーターのチュートリアル
description: ' [!DNL Adobe Workfront Fusion] でルーターを使用して、ポケモンとスーパーヒーローのバンドルを正しいパスに渡す方法を学びます。'
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9013
exl-id: 6c111e5b-1c8f-43fd-9e2d-16599de2a337
recommendations: noDisplay,catalog
doc-type: video
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: ht
source-wordcount: '853'
ht-degree: 100%

---

# ルーターのチュートリアル

ルーターを使用して、正しいパスにポケモンとスーパーヒーローのバンドルを渡し、各キャラクターのタスクを作成します。

![Fusion シナリオの画像](assets/universal-connectors-and-routing-2.png)

## ルーターのチュートリアル

Workfront では、独自の環境で演習を再現する前に、演習のチュートリアルのビデオを見ることをお勧めします。

>[!VIDEO](https://video.tv.adobe.com/v/3416573/?quality=12&learn=on&enablevpops&captions=jpn)

## 演習 URL

* スーパーヒーロー API Web サイト： `https://www.superheroapi.com/`
* 演習の最初の URL：`https://www.superheroapi.com/api/{access-token}/{character-id}/appearance`
* 演習の 2 番目の URL：`https://www.superheroapi.com/api/{access-token}/{character-id}/powerstats`

独自のスーパーヒーロートークンへのアクセスで問題が発生した場合は、共有トークン「10110256647253588」を使用できます。スーパーヒーロー API の呼び出し回数に気を配って、この共有トークンが引き続き全員に対して機能するようにしてください。



## マッピングパネルで項目を検索する

マッピングパネルの上部にある「項目を検索」フィールドを使用すると、フィールドが配列内にネストされている場合でも、パネル内のフィールドをすばやく見つけることができます。検索では、大文字と小文字が区別されません。

![最初の検索パネルの画像](assets/universal-connectors-and-routing-3.png)

![2 番目の検索パネルの画像](assets/universal-connectors-and-routing-4.png)

## API を使用する際のヒントとテクニック

これまで、シナリオで必要な情報を取り込むために追加の認証を必要としない、非常にシンプルな API（アプリケーションプログラミングインターフェイス）を使用して作業しました。 API やユニバーサルコネクタを使用する際に役立つヒントを以下に示します。

## 手順 1：API のタイプを特定する

Workfront や多くのソフトウェアシステムは、現在最も簡単で最も標準的なタイプの API である REST（Representational State Transfer）API を使用して構築されています。 ただし、その他にも、次のようなものがあります。

* SOAP（Simple Object Access Protocol）（Workfront の Proof API は SOAP ベース）
* FTP（ファイル転送プロトコル）
* SFTP（セキュアファイル転送プロトコル）
* 詳しくは、Web 検索を実行して、API タイプと興味のあるキーワードを確認してください。

>[!NOTE]
>
>Salesforce などの大規模なプラットフォームに接続する場合、プラットフォームの異なるエリアで異なる API が提供されます。 接続先のサービスに適したサービスが見つかっていることを確認します。

## 手順 2：API で必要な認証のタイプを特定する

API 認証は、Workfront Fusion を通じて接続しようとする場合など、サービスへのアクセスを制御するために使用される識別形式です。これは、システムへのアクセスが許可されていることを別のシステムに証明するのに役立ちます。 OAuth 2 は、現在使用されている最も一般的な認証タイプです。 API 認証に関するインターネット検索の詳細を説明します。

認証は、API を使用する場合の最も難しい側面になる可能性があります。 Workfront Fusion のユニバーサルコネクターの最も役に立つ機能の 1 つは、OAuth 2、API キーなどの基本認証などの一般的な認証方法を使用する場合に、Workfront Fusion が認証を処理できる点です。認証方法（OAuth 2 など）に適した Workfront Fusion モジュールを使用して接続を作成すると、Workfront Fusion は、シナリオを実行するたびに API キーやトークンを継続的に生成します。

Experience League に関する拡張認証の概要記事で、Workfront が提供する様々な種類の認証について説明します。

## 手順 3：API ドキュメントを読み、必要なエンドポイントを見つける

API が別のシステムとやり取りする場合、この通信のタッチポイントはエンドポイントと見なされます。エンドポイントとは、API がリクエストを送信する場所と、リソースが存在する場所です。

ユニバーサルコネクタを使用して API を操作する場合、API がサポートするエンドポイントと、各リクエストに必要なデータを理解する必要があります。 API ドキュメントでは、API のエンドポイントと、作成、読み取り、更新、削除などの一般的な操作の実行方法を説明する必要があります。これらの呼び出しを実行するには、特に API 呼び出しを行うことが初めての場合や、新しい API を使用する場合などは、ある程度の練習が必要です。

Workfront Fusion Universal Connectors の詳細と、Experience League で必要な API に接続するための設定方法について説明します。

## 最終メモ

Experience League で、事前定義済みのアプリコネクタの完全なリストを確認できます。 新しいアプリコネクタを Workfront Fusion 製品チームに提案するには、アイデアをイノベーションラボに送信してください。 送信するのが初めての方は、イノベーションラボの詳細に加えて、年 2 回のリーダーボードの優先順位付けにアイデアに投票し、参加する方法をご覧ください。既にイノベーションラボにアクセスできる場合は、ログインしてアイデアを送信してください。

## やってみよう

>[!NOTE]
>
>練習の演習や課題は任意で、Fusion トレーニングを完了するのに必須ではありません。

この練習は、チュートリアルで学習した内容に基づいて構築されますが、ソリューションは提供されていません。

ポケモンキャラクター用の「複数の変数を設定」モジュールで、「Stat（Level）」という名前の変数を作成します。この変数にポケモンの統計の名前をマッピングします。 配列値機能を使用して、配列の表示方法を変更し、各統計が以下のように新しい行になるようにします。

**ヒント**： 対応するレベルのポケモンの統計は 6 種類しかありません。

![統計の画像](assets/universal-connectors-and-routing-5.png)

**課題**：値の文字列をコンマで区切って表示するのではなく、上記のように、配列の数式を使用して「能力」を別の行に表示できるかを確認してください。下のスクリーンショットにヒントがあります。

![配列名の画像](assets/universal-connectors-and-routing-6.png)

## 詳細情報 以下をお勧めします。

[Workfront Fusion ドキュメント](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=ja)
