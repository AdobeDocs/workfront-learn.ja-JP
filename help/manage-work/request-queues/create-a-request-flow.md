---
title: Workfrontでのリクエストフローの作成
description: 効率的な割り当てのルーティングルールを作成し、ネストされたトピックグループを使用してリクエストを整理し、キュートピックをワークフローにリンクし、リクエストフローの機能をテストし、正確性と効率を確保する柔軟な調整を行うことで、リクエスト管理を最適化します。
activity: deploy
feature: Work Management
type: Tutorial
role: Admin, User
level: Intermediate
team: Technical Marketing
thumbnail: 335223.jpeg
jira: KT-8960
last-substantial-update: '2024-09-11T00:00:00.000Z'
recommendations: noDisplay,catalog
exl-id: 194df349-541d-4940-a6a5-b5d47cb58cf4
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: c10f2e93-7a58-4212-aa24-684c265ebe76
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-06T14:41:59.860Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 400
ht-degree: 29%

---

# Workfrontでのリクエストフローの作成

>[!PREREQUISITES]
>
>* [リクエストキューの作成](/help/manage-work/request-queues/create-a-request-queue.md)
>* [リクエストフローの設定について](/help/manage-work/request-queues/understand-settings-for-a-flow-request.md)

このビデオでは、キューのトピック、トピックグループ、ルーティングルールを設定して、リクエストフローを作成する手順を説明します。 &#x200B; プロセスは、リクエストの割り当て方法を定義するルーティングルールの作成から始まります。&#x200B;次に、トピックグループを作成してリクエストを整理します。&#x200B;これらのグループはキューに追加でき、作成できるトピックグループの数に制限はありません。
次に、ビデオでは、ルーティングルール、トピックグループ、カスタムフォーム、承認プロセス、デフォルトの期間にリンクされるキュートピックを作成する方法について説明します。
最後に、ビデオでは、正しくルーティングされていることを確認するためにリクエストを送信して設定をテストする方法を示します。 &#x200B;問題が発生した場合は、キューを調整できます。 &#x200B;このビデオでは、適切なルーティングと整理を確保するために、リクエストフローの構造と機能を検証することの重要性を強調しています。

>[!VIDEO](https://video.tv.adobe.com/v/335223/?quality=12&learn=on&enablevpops=0)

## 重要な留意点

* **ルーティングルールの設定：** ルーティングルールは、リクエストの割り当て方法を、チーム（Creative チームなど）または個人（Jennifer CampbellやMark Lewisなど）のいずれに対しても決定します。 &#x200B;これらのルールは、ルールに名前を付け、説明を追加し、デフォルトの担当者またはチームを選択して作成します。
* **トピックグループの作成：** トピックグループは、「デジタル」や「印刷」などのカテゴリにリクエストを整理するのに役立ちます。 &#x200B;作成できるトピックグループの数に制限はなく、最大10 レベルまでネストできます。
* **キューのトピック設定：** キューのトピックは、ルーティングルール、トピックグループ、カスタムフォーム、承認プロセス、およびデフォルトの期間にリンクされています。 &#x200B;例えば、「パンフレット」という名前のキュートピックをプリントトトトピックグループに関連付けて、Creative チームにルーティングできます。
* **リクエストフローのテスト：** リクエストキューを設定した後、適切なルーティングと機能を確保するためにリクエストを送信してフローをテストすることが重要です。 &#x200B; キューの設定を再確認することで、問題を解決できます。 &#x200B;
* **調整の柔軟性：**&#x200B;システムでは、問題が発生した場合にルーティングルール、トピックグループ、キュートピックを変更できるので、リクエストフローが効率的で正確であることが確保されます。


## このトピックに関する推奨チュートリアル

* [システム管理者のフィードバックリクエストキューの作成](/help/manage-work/request-queues/create-a-system-admin-feedback-request-queue.md)
* [リクエストキューに関するよくある質問へ回答](/help/manage-work/request-queues/request-queue-faq.md)


