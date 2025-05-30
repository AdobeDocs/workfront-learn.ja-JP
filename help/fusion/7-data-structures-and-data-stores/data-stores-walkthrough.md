---
title: データストアのチュートリアル
description: ' [!DNL Adobe Workfront Fusion] で、データストアを使用して、企業リストと Workfront 間で企業名を同期させる方法について説明します。'
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9055
exl-id: e96fd109-2463-4702-b1bf-b42a6dcd7fc4
recommendations: noDisplay,catalog
doc-type: video
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: ht
source-wordcount: '393'
ht-degree: 100%

---

# データストアのチュートリアル

この演習では、データストアを使用して、企業リストと Workfront 間で企業名を同期させます。

これは、Workfront と他のシステムの企業を一方向の同期させるための 1 つのパーツです。現時点では、CSV ファイルと Workfront の間でのみ同期できます。ただし、各会社の CSV ファイル（CID）内に Workfront ID（WFID）と会社 ID を管理するテーブルをデータストアに保持します。これにより、将来的には双方向の同期を実現できる予定です。

![Fusion シナリオの画像](assets/data-structures-and-data-stores-2.png)

## データストアのチュートリアル

Workfront では、独自の環境で演習を再現する前に、演習のチュートリアルのビデオを見ることをお勧めします。

>[!VIDEO](https://video.tv.adobe.com/v/3417971/?quality=12&learn=on&enablevpops&captions=jpn)



## 最終メモ

これでデータ構造とデータストアについて理解したので、今度は「それをいつ使用すべきか」という疑問が湧くかもしれません。

データ構造は、JSON、XML、CSV などのデータ形式をシリアル化したり、解析したりするために一般的によく使用されます。データ構造を使用すると、データの構造を制御したり、データを検証したりできます。データ構造を使用する最も一般的な理由は、JSON や XML を期待する API に、有効なデータを作成して送信するためです。このような場合、JSON アプリまたは XML アプリをデータ構造と共に使用して、データが正しい形式であることを確認する必要があります。

データストアは、複数のシナリオの実行でアクセスする必要がある、永続的なデータの保存にのみ使用する必要があります。例えば、処理を正確に制御する必要がある高度なユースケースのために、最後に処理されたレコードに関するメタデータを保存できます。

データストアは、データウェアハウスまたはログとして使用するように設計されていません。データストアには Workfront Fusion 以外ではアクセスできず、データストアとのほとんどのやり取りは Workfront Fusion のシナリオを通じて行われます。その結果、データウェアハウスやログのユースケースで想定されるような分析またはレポートツールにデータストアを接続することはできません。このようなユースケースにおける Workfront Fusion の役割は、データの整理と保存に適したシステム（SQL、MariaDB など）を実装することです。

## 詳細情報 以下をお勧めします。

[Workfront Fusion ドキュメント](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=ja)
