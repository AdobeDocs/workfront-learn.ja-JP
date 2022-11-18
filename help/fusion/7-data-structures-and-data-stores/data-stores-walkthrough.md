---
title: データストアのチュートリアル
description: を使用して、会社のリストとWorkfrontの間で会社名を同期する方法を説明します。 [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: Jira ticket
exl-id: e96fd109-2463-4702-b1bf-b42a6dcd7fc4
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# データストアのチュートリアル

## 概要

この演習では、データストアを使用して、会社のリストとWorkfrontの間で会社名を同期します。

これは、Workfrontや他のシステムにおける、企業の一方向の同期の一環です。 現時点では、CSV ファイルとWorkfrontの間でのみ同期されます。 また、データストアにテーブルを保持して、各会社のWorkfront ID(WFID) と CSV ファイル (CID) での会社 ID を追跡します。 これにより、将来のある時点で双方向の同期を実現できます。

![Fusion シナリオのイメージ](assets/data-structures-and-data-stores-2.png)

## データストアのチュートリアル

Workfrontは、独自の環境で演習を再作成する前に、演習のチュートリアルのビデオを見ることをお勧めします。

>[!VIDEO](https://video.tv.adobe.com/v/335296/?quality=12)

>[!TIP]
>
>チュートリアルの完了手順については、 [データストアのチュートリアル](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/data-stores.html?lang=en) 運動。


## 最終メモ

データ構造とデータストアの学習が完了したので、「いつ使用すべきか」と自問するかもしれません。

データ構造は、JSON、XML、CSV などのデータ形式のシリアル化や解析に最も一般的に使用されます。 データ構造を使用すると、データの構造を制御したり、データを検証したりできます。 データ構造を使用する最も一般的な理由は、JSON または XML を想定する API に送信する有効なデータを作成することです。 このような場合、JSON アプリまたは XML アプリをデータ構造と共に使用して、データが正しい形式であることを確認します。

データストアは、複数のシナリオの実行でアクセスする必要がある永続的なデータの保存にのみ使用する必要があります。 例えば、処理を正確に制御する必要がある高度なユースケース向けに処理された最後のレコードに関するメタデータを保存できます。

データストアは、データウェアハウスまたはログとして使用するように設計されていません。 データストアにはWorkfront Fusion 以外ではアクセスできず、データストアとのほとんどのやり取りはWorkfront Fusion シナリオを通じておこなわれます。 その結果、データストアを、Data Warehouse およびログの使用例で期待される分析またはレポートツールに接続することはできません。 Workfront Fusion の役割は、このような使用例では、データ（SQL、MariaDB など）の整理と保存に適したシステムを設定することです。

## 詳細情報 以下をお勧めします。

[Workfront Fusion ドキュメント](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
