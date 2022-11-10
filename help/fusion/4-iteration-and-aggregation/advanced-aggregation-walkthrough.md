---
title: 高度な集計のチュートリアル
description: Web サービスを呼び出して、複数の国に関する詳細を返し、サブ地域ごとにグループ化された母集団を識別する方法を、 [!DNL Adobe Workfront Fusion].
activity: use
doc-type: feature video
team: Technical Marketing
kt: Jira ticket
exl-id: c79250d0-7341-4a25-83dc-de99ce5c6dc4
source-git-commit: ca56810c9eab36175a6280e319b5fd2aba90b2f2
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# 高度な集計のチュートリアル

## 概要

Web サービスを呼び出して複数の国に関する詳細を返し、すべての国の総母集団をサブ地域ごとにグループ化します。

![Fusion シナリオのイメージ](assets/iteration-and-aggregation-3.png)

## 高度な集計のチュートリアル

Workfrontは、独自の環境で演習を再作成する前に、演習のチュートリアルのビデオを見ることをお勧めします。

>[!VIDEO](https://video.tv.adobe.com/v/335281/?quality=12)

## 演習 URL

* `https://restcountries.com/v2/lang/es`
* `https://restcountries.com/v2/name/{country name}`

>[!TIP]
>
>チュートリアルの完了手順については、 [高度な集計のチュートリアル](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/advanced-aggregation.html?lang=en) 運動。

## 集合原理の強化

モジュールが複数のバンドルを出力するたびに、その後の各モジュールが各バンドルを実行します。

これを防ぐには、複数のバンドルを生成する可能性があるモジュールの後に集約を追加します。

シナリオ内の任意のセグメントを囲むシャドウが、 **beginning-iterator** から **終了集約**. これにより、これらのセグメントをWorkfront Fusion シナリオで見つけやすくなります。

## あなたのターン

この練習は、チュートリアルで学習した内容に基づいて構築されますが、ソリューションは提供されていません。

新しいシナリオを作成して、マーケティングポートフォリオのプロジェクトでログオンしたタスクをすべて合計します。 次に、「{ プロジェクト名 } のプロジェクトチームが、{ 計画時間 } 計画時間の合計 {summed hours} 時間をログに記録し、計画の {percentage} に表示した」というメールを 1 通送信します。

**課題：** 今年のログに記録された時間だけ同じことができるかどうかを確認します。

## 詳細情報 以下をお勧めします。

[Workfront Fusion ドキュメント](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
