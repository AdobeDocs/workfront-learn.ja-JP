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
autotag-review: '2026-05-06T16:33:27.197Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 258
ht-degree: 100%

---

# 高度な集計のチュートリアル

Web サービスを呼び出して複数の国に関する詳細を返し、サブ地域ごとにグループ化されたすべての国の総人口を特定します。

![Fusion シナリオの画像](assets/iteration-and-aggregation-3.png)

## 高度な集計のチュートリアル

Workfront では、独自の環境で演習を再現する前に、演習のチュートリアルのビデオを見ることをお勧めします。

>[!VIDEO](https://video.tv.adobe.com/v/3417305/?captions=jpn&quality=12&learn=on&enablevpops=1)

## 演習 URL

* `https://restcountries.com/v2/lang/es`
* `https://restcountries.com/v2/name/{country name}`



## 集計原理の強化

モジュールが複数のバンドルを出力するたびに、その後のすべてのモジュールが各バンドルを実行します。

これを防ぐには、複数のバンドルを生成する可能性があるモジュールの後に集計を追加します。

シナリオ内の任意のセグメントを囲むシャドウが、**beginning-iterator** から **ending-aggregator** まで表示されます。 これにより、これらのセグメントを Workfront Fusion シナリオで見つけやすくなります。

## やってみよう

>[!NOTE]
>
>練習の演習や課題は任意で、Fusion トレーニングを完了するのに必須ではありません。

この練習は、チュートリアルで学習した内容に基づいて構築されますが、ソリューションは提供されていません。

新しいシナリオを作成して、マーケティングポートフォリオのプロジェクトのタスクにログオンしたすべての時間を合計します。 次に、「{Project Name} プロジェクトチームが、合計 {planned hours} 時間の予定時間数のうち {summed hours} 時間をログに記録し、計画の {percentage} ％に達しています」というメールを 1 通送信します。

**課題：**&#x200B;同じことを、ログに記録された時間を今年のみに限ってできるかどうかを試してください。

## 詳細情報 以下をお勧めします。

[Workfront Fusion のドキュメント](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
