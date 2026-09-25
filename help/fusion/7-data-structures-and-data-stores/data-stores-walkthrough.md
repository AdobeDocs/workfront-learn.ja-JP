---
title: データストアのチュートリアル
description: '[!DNL Adobe Workfront Fusion]を使用して企業一覧とWorkfront間で企業名を同期する方法について説明します。'
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
autotag-review: '2026-05-06T16:18:10.872Z'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
    internal-label: Workfront Fusion
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
source-git-commit: 54883ad8c8df3aaee06ba8f8dca64227594c1c77
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 95%
---
# データストアのチュートリアル

この演習では、データストアを使用して、企業リストと Workfront 間で企業名を同期させます。

これは、Workfront と他のシステムの企業を一方向の同期させるための 1 つのパーツです。 現時点では、CSV ファイルと Workfront の間でのみ同期できます。 ただし、各会社の CSV ファイル（CID）内に Workfront ID（WFID）と会社 ID を管理するテーブルをデータストアに保持します。 これにより、将来的には双方向の同期を実現できる予定です。

![Fusion シナリオの画像](assets/data-structures-and-data-stores-2.png)

## データストアのチュートリアル

Workfront では、独自の環境で演習を再現する前に、演習のチュートリアルのビデオを見ることをお勧めします。

>[!VIDEO](https://video.tv.adobe.com/v/335296/?quality=12&learn=on&enablevpops=1)



## 最終メモ

これでデータ構造とデータストアについて理解したので、今度は「それをいつ使用すべきか」という疑問が湧くかもしれません。

データ構造は、JSON、XML、CSV などのデータ形式をシリアル化したり、解析したりするために一般的によく使用されます。 データ構造を使用すると、データの構造を制御したり、データを検証したりできます。 データ構造を使用する最も一般的な理由は、JSON や XML を期待する API に、有効なデータを作成して送信するためです。 このような場合、JSON アプリまたは XML アプリをデータ構造と共に使用して、データが正しい形式であることを確認する必要があります。

データストアは、複数のシナリオの実行でアクセスする必要がある、永続的なデータの保存にのみ使用する必要があります。 例えば、処理を正確に制御する必要がある高度なユースケースのために、最後に処理されたレコードに関するメタデータを保存できます。

データストアは、データウェアハウスまたはログとして使用するように設計されていません。 データストアには Workfront Fusion 以外ではアクセスできず、データストアとのほとんどのやり取りは Workfront Fusion のシナリオを通じて行われます。 その結果、データウェアハウスやログのユースケースで想定されるような分析またはレポートツールにデータストアを接続することはできません。 このようなユースケースにおける Workfront Fusion の役割は、データの整理と保存に適したシステム（SQL、MariaDB など）を実装することです。

## 詳細情報 以下をお勧めします。

[Workfront Fusion のドキュメント](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
