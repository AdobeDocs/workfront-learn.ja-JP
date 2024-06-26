---
title: メールアラートとプルーフ通知について
description: ' [!DNL  Workfront]のメールアラートとプルーフ通知の違いについて。'
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: email-alert-vs-proof-notifications.png
jira: KT-10174
last-substantial-update: 2024-01-24T00:00:00Z
exl-id: 51423110-960c-46ed-8b4e-6e73c67c42e0
source-git-commit: 30748311c14fb8aa6b10c03a74e83f46bdb5dfbf
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 100%

---

# メールアラートとプルーフ通知について

メールアラートは、プルーフ通知メールとは異なります。レビュー対象の新しいプルーフが割り当てられた際、プルーフが遅れた際、または新しいバージョンのプルーフが表示された際に、プルーフ通知メールを受け取ります。

![レビューする新しいプルーフがあることを示すプルーフ通知メールの画像。](assets/email-alert-1.png)

プルーフのアップロード時に通知オプションをオフにした場合、レビューする新しいプルーフがあるという連絡を、誰も [!DNL Workfront] から受け取りません。

ほとんどの場合、プルーフがアップロードされると、メールアラートはレビュー担当者や承認者ごとに設定されます。プルーフの受信者には、デフォルトのメールアラートプルーフをアップロードするたびに設定する必要がないように、デフォルトのメールアラートタイプがプルーフの受信者に割り当てられている場合があります。これらのデフォルト設定の取得については、システム管理者にお問い合わせください。

![プルーフに対する決定が下され、レビューするコメントがあることを示すメールアラートの画像。](assets/email-alert-2.png)

メールアラートが[!UICONTROL 無効]に設定された場合でも、プルーフの受信者には、新しいプルーフやバージョンが通知されます。

## ベストプラクティス

| ベストプラクティス | その理由は次のとおりです |
|---|---|
| Workfront 設定の「プルーフにコメントが作成されたら Workfront からメールを送信する」設定を無効にします。 | この設定が有効になっている場合（デフォルトでは有効）、ユーザーはプルーフに関するコメントごとに複数のメール通知（1 つはプルーフ機能から、もう 1 つは Workfront 自体から）を受信する可能性があります。このように通知が重複すると、メール通知の中断と混乱や、メールのインボックスがいっぱいになることにつながり、最終的にユーザーが受信したプルーフ通知を無視してしまい、期限を逃してしまうことがあります。<br> <br>メモ：この設定は、Workfront メインメニュー／設定／メール／レビューと承認にあります。 |


