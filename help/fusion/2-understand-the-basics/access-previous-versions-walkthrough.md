---
title: 以前のバージョンへのアクセスのチュートリアル
description: シナリオに変更を加えて  [!DNL Adobe Workfront Fusion] に保存した後、以前のバージョンを復元する方法を説明します。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9009
exl-id: dd2cc2a2-e5af-41cc-bc0d-6be1efd996d9
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
autotag-review: '2026-05-06T16:39:17.503Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 280
ht-degree: 100%

---

# 以前のバージョンへのアクセスのチュートリアル

このビデオでは、次の操作を実行します。

* シナリオに変更を加えて複数回保存した後、以前のバージョンを復元する方法を説明します。

## 以前のバージョンへのアクセスの手順

Workfront では、独自の環境で演習を再現する前に、演習のチュートリアルのビデオを見ることをお勧めします。

>[!VIDEO](https://video.tv.adobe.com/v/3416537/?captions=jpn&quality=12&learn=on&enablevpops=1)

>[!NOTE]
>
>シナリオを保存した後、将来アクセスする必要がある場合、「...」メニューから新しいバージョンを使用できます。 以前に保存したシナリオのバージョンは 60 日間のみ使用できます。 監査目的で 60 日を超える以前のバージョンにアクセスする必要がある場合、Workfront では、シナリオのブループリントを保存し、同意された場所にアーカイブすることをお勧めします。


## 用語の追加

![監視レコードとカスタム web フックモジュールの画像](assets/understand-the-basics-3.png)

### トリガーモジュール

トリガーモジュールは、最初のモジュールとしてのみ使用でき、0 個、1 個または複数のバンドルを返すことができます。 これらは、集約されない限り、後続のモジュールで個別に処理されます。

**ポーリングトリガー（トリガー時に時計）** - 最後に処理されたレコードを追跡するための特別な機能。

**インスタントトリガー（トリガー時に稲妻）** - Webhook に基づいて、直ちにトリガーされます。

![レコード作成とモジュール検索の画像](assets/understand-the-basics-4.png)

### アクションと検索モジュール

**アクション** - CRUD（作成、読み取り、更新、削除）操作の実行に使用

**検索** - 0 個、1 個または複数のレコードを検索し、それらをバンドルとして返します。これは、集約しない限り、後続のモジュールで個別に処理されます。

## 詳細情報 以下をお勧めします。

[Workfront Fusion のドキュメント](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
