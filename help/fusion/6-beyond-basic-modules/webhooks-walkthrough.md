---
title: Webhooks のチュートリアル
description: Webhook を使用してアプリを作成し、顧客がお酒を購入するのに十分な年齢かどうかを判断する方法を説明します ( [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9051
exl-id: 7870c9db-d538-440a-8972-e7bc5ac5af93
source-git-commit: 0618bf27478744e0e9976015a24c5ec8519efbb7
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# Webhooks のチュートリアル

## 概要

このシナリオでは、コンビニエンスストアのアプリを作成して、顧客がお酒を買うのに十分な年齢かどうかを簡単に判断できるようにします。 レジでは、顧客の名前と誕生日、および確認済みのクライアントトークンを、提供された URL に投稿する必要があります。 入力すると、シナリオがトリガーされ、適切な応答を計算して要求者に返します。

![スイッチモジュールを使用した画像](assets/beyond-basic-modules-5.png)

## Webhooks のチュートリアル

Workfrontは、独自の環境で演習を再作成する前に、演習のチュートリアルのビデオを見ることをお勧めします。

>[!VIDEO](https://video.tv.adobe.com/v/335292/?quality=12)

>[!TIP]
>
>チュートリアルの完了手順については、 [Webhooks のチュートリアル](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/webhooks.html?lang=en) 運動。

## Postman設定

チュートリアルの演習に従うには、無料のPostmanアプリケーションをダウンロードする必要があります。 この演習では、Postmanの適切な領域に移動するには、次の手順に従います。

1. ワークスペースを作成し、開きます。
1. 「新規」タブをクリックし、「飲酒年齢」という名前の新しいコレクションを作成します。
1. 「新規」タブを再度クリックし、「GETの生成日」という名前の新しいGETリクエストを作成します。
1. リクエストアクションをGETからPOSTに変更します。
1. 「POSTURL 」フィールドの下の「本文」サブタブ領域に移動します。
1. 「認証」サブタブの下で「 form-data 」を選択します。
1. 名前、誕生日、clientToken の 3 つのキーを作成します。

![スイッチモジュールを使用した画像](assets/beyond-basic-modules-6.png)

## あなたのターン

>[!NOTE]
>
>練習の演習や課題は任意で、Fusion トレーニングを完了するのに必要ではありません。

この練習は、チュートリアルで学習した内容に基づいて構築されますが、ソリューションは提供されていません。

作成された新しい更新を待機しているWorkfrontの Webhook を作成し、日付、更新をおこなった人の名前、更新内容を記録します。 この情報を自分に電子メールで送信します。

**ヒント**:Workfront Watch Eventsトリガーモジュールを使用して、Webhook を作成します。 また、Workfrontでは、更新をメモと呼びます。

**課題**:更新が行われた場所の URL を見つけて追加し、アクセスしやすくしますか？


## 詳細情報 以下をお勧めします。

[Workfront Fusion ドキュメント](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
