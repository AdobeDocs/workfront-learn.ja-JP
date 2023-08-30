---
title: Webhook
description: Webhook で開始されるシナリオを作成、トリガー、管理する方法について説明します。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11053
thumbnail: KT11053.png
exl-id: d6a62a26-a8ab-477c-a8f2-98f3b9ff5edf
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '647'
ht-degree: 100%

---

# Webhook

Webhook で開始されるシナリオを作成、トリガー、管理する方法について説明します。

## 演習の概要

このシナリオの目的は、コンビニエンスストアに販売するアプリを作成して、お客様がアルコールを購入できる年齢に達しているかどうかをコンビニエンスストアが簡単に判断できるようにすることです。レジ担当者は、お客様の名前と生年月日を、提供された URL に POST するだけで済みます。その POST によって、回答を計算してリクエスターに返すシナリオがトリガーされます。

1. このシナリオは、3 つの Webhook で構成されています。
1. トリガーモジュールは、POST をリッスンするカスタム Webhook です。
1. POST を受信すると、次のモジュールの 1 つに出力されます。
1. 次のモジュールは、リクエスターに応答を返します。

   ![Webhook 画像 1](../12-exercises/assets/webhooks-walkthrough-1.png)

## 手順

**トリガー Webhook を設定します。**

1. 新しいシナリオを作成し、「Webhook の使用」という名前を付けます。
1. トリガーには、Webhook アプリからカスタム Webhook モジュールを追加します。
1. 「追加」をクリックして、新しい Webhook を作成します。
1. 「飲酒年齢アプリ」の Webhook 名を入力します。
1. IP 制限は空白のままにします。つまり、誰でもデータを送信できます。
1. 「保存」をクリックします。


   ![Webhook 画像 2](../12-exercises/assets/webhooks-walkthrough-2.png)

1. Webhook マッピングパネルに戻ると、この特定の Webhook 用の URL が作成されます。「アドレスをクリップボードにコピー」をクリックして、その URL をコピーします。
1. 「OK」をクリックします。
1. 「1 回実行」をクリックします。
1. Postman で URL を使用して、名前と生年月日をカスタム Webhook に送信します。Postman の設定手順については、[Webhook のチュートリアル](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/beyond-basic-modules/webhooks-walkthrough.html?lang=ja)を参照してください。

   **Webhook モジュールパネルは次のようになります。**

   ![Webhook 画像 3](../12-exercises/assets/webhooks-walkthrough-3.png)

   **Webhook は、データ構造を判断するためにデータをリッスンしている状態になりました。**

1. 取得するペイロードのデータ構造を定義できます（データ構造については後で説明します）。 データ構造を定義していない場合、Fusion は、POST の送信時にデータ構造を自動的に決定します。
1. Postman 側では、コピーした URL に送信します。投稿には、基本的なフォームデータが含まれている必要があります。この例では、名前、生年月日、clientToken の 3 つのフィールドが必要です。

   ![Webhook 画像 4](../12-exercises/assets/webhooks-walkthrough-4.png)

1. 「Postman から送信」をクリックすると、POST が承認されたことを示すメッセージが表示されます。
1. これは、シナリオで、データ構造が正常に決定されたことを示すポイントです。
1. 実行インスペクターを開くと、データが受信されたことを確認できます。

   ![Webhook 画像 5](../12-exercises/assets/webhooks-walkthrough-5.png)

   **クライアントトークンのルーティングを設定します。**

1. ルーターをトリガーモジュールに追加します。
1. 上部のパスに Webhook 応答モジュールを追加します。これは、クライアントトークンが一致しない場合のパスになります。
1. ステータスを 401 に設定します。
1. 本文を {&quot;エラー&quot; : &quot;リクエストの認証に失敗しました。clientToken を確認してください&quot;} に設定します。

   ![Webhook 画像 6](../12-exercises/assets/webhooks-walkthrough-6.png)

1. ルーターと Webhook 応答モジュールの間にフィルターを作成します。「クライアントトークンが一致しません」という名前を付けます。
1. 条件には、トリガーモジュールの clientToken フィールドを使用し、「次に等しくない」を使用して、5121933 と数値比較を行います。

   ![Webhook 画像 7](../12-exercises/assets/webhooks-walkthrough-7.png)

1. 下部のパスに別の Webhook 応答モジュールを追加します。 これは、クライアントトークンが一致する場合のパスになります。
1. ステータスを 200 に設定します。
1. 本文の設定では、マッピングパネルの関数を使用して、ユーザーが 21 歳以上かどうかをテストします。そうであれば「あんたは飲酒が可能な年齢です」、そうでなければ「残念ですが…」を返します。

   ![Webhook 画像 9](../12-exercises/assets/webhooks-walkthrough-9.png)

1. ルーターと下位パスの Webhook 応答モジュールの間にフィルターを作成します。「クライアントトークンが一致します」という名前を付けます。
1. 条件には、トリガーモジュールの clientToken フィールドを使用し、5121933 という数値と「次に等しい」比較を行います。


   ![Webhook 画像 8](../12-exercises/assets/webhooks-walkthrough-8.png)

1. 「1 回実行」の下にある 「スケジュール」ボタンをクリックしてシナリオをアクティブ化し、新しい投稿があるたびに受信され、いずれかのパスをたどって応答を生成するようにします。
