---
title: 高度な集計のチュートリアル
description: ' [!DNL Adobe Workfront Fusion]で web サービスを呼び出して、複数の国に関する詳細を返し、サブ地域ごとにグループ化された人口を特定する方法を説明します。'
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9040
exl-id: c79250d0-7341-4a25-83dc-de99ce5c6dc4
recommendations: noDisplay,noCatalog
doc-type: video
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 100%

---

# 高度な集計のチュートリアル

Web サービスを呼び出して複数の国に関する詳細を返し、サブ地域ごとにグループ化されたすべての国の総人口を特定します。

![Fusion シナリオの画像](assets/iteration-and-aggregation-3.png)

## 高度な集計のチュートリアル

Workfront では、独自の環境で演習を再現する前に、演習のチュートリアルのビデオを見ることをお勧めします。

>[!VIDEO](https://video.tv.adobe.com/v/335281/?quality=12&learn=on)

## 演習 URL

* `https://restcountries.com/v2/lang/es`
* `https://restcountries.com/v2/name/{country name}`



## 集計原理の強化

モジュールが複数のバンドルを出力するたびに、その後のすべてのモジュールが各バンドルを実行します。

これを防ぐには、複数のバンドルを生成する可能性があるモジュールの後に集計を追加します。

シナリオ内の任意のセグメントを囲むシャドウが、**beginning-iterator** から **ending-aggregator** まで表示されます。これにより、これらのセグメントを Workfront Fusion シナリオで見つけやすくなります。

## やってみよう

>[!NOTE]
>
>練習の演習や課題は任意で、Fusion トレーニングを完了するのに必須ではありません。

この練習は、チュートリアルで学習した内容に基づいて構築されますが、ソリューションは提供されていません。

新しいシナリオを作成して、マーケティングポートフォリオのプロジェクトのタスクにログオンしたすべての時間を合計します。次に、「{Project Name} プロジェクトチームが、合計 {planned hours} 時間の予定時間数のうち {summed hours} 時間をログに記録し、計画の {percentage}％に達しています」というメールを 1 通送信します。

**課題：**&#x200B;同じことを、ログに記録された時間を今年のみに限ってできるかどうかを試してください。

## 詳細情報 以下をお勧めします。

[Workfront Fusion ドキュメント](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=ja)
