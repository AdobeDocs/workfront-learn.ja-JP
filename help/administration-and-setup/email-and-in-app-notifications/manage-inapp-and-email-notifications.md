---
title: アプリ内イベントおよび電子メールイベント通知の管理
description: ユーザーが受け取るアプリ内通知と電子メール通知を制御して、作業に関して関連性の高い有用な電子メールを受け取る方法を説明します。
short-description: Learn how users can control which in-app and email notifications they receive.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner
thumbnail: 10095.jpeg
kt: 10095
exl-id: 831646d2-ecf8-4fe6-8d4e-8c5fc233ed56
source-git-commit: fca5e76133ef0a81aa6063d71baf5500646dbe1e
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 8%

---

# アプリ内および電子メールイベント通知の管理

E メールは日常生活の一部であり、数日の間に、得られる E メールの量は圧倒的です。 ただし、 [!DNL Workfront]を使用すると、システム管理者は、関連する作業に関する関連性の高い便利な電子メールを全員が確実に受け取るようにできます。

Workfrontからユーザーに送信できる通知には、いくつかのタイプがあります。 これらの通知の一部はシステムレベルで制御され、すべてのユーザーに影響を与えます。 一部の通知は、1 日のダイジェストで即座に E メールを生成するように設定できます。 または、E メールをオフにして、Workfront内での通知のみを生成します。

## イベント通知

イベントとは、ステータスの変更、投稿されたコメント、または行われた割り当てのようなもので、でアプリ内通知をトリガーできます。 [!DNL Workfront].

![通知リスト](assets/admin-fund-user-notifications-01.png)

ただし、環境設定のオプションを選択または選択解除することで、電子メール通知を受け取るイベントを決定できます。

これらの変更を行うには、 [!UICONTROL メインメニュー].

![のユーザー名 [!UICONTROL メインメニュー]](assets/admin-fund-user-notifications-02.png)

クリック [!UICONTROL 編集] から [!UICONTROL 詳細] メニュー

![ユーザープロファイルページのメニュー](assets/admin-fund-user-notifications-03.png)

クリック [!UICONTROL 通知] 内 [!UICONTROL 担当者の編集] ポップアップボックス。

![[!UICONTROL 担当者の編集] window](assets/admin-fund-user-notifications-04.png)

ここから、即座に受信する通知、毎日受信する通知、まったく受信しない通知を決定できます。 ここで行った変更は、ユーザーに固有のもので、Workfrontの他のユーザーには影響しません。

**[!UICONTROL 日次]**

デフォルトでは、E メールは即座に送信されるように設定されています。 ただし、電子メール通知の頻度を [!UICONTROL 即時] から [!UICONTROL 毎日]必要な情報が必要に応じて得られるようにします。

![[!UICONTROL 通知] セクション [!UICONTROL 担当者の編集] window](assets/admin-fund-user-notifications-05.png)

「毎日」オプションを選択すると、その日のイベントのダイジェストが 1 通の電子メールで送信されます。 ユーザーには、 [!UICONTROL 通知] 」セクションに入力します。

例えば、 [!UICONTROL 所有するプロジェクトに関する情報] セクションは、1 日に 1 件の E メールを生成します。 [!UICONTROL 必要なアクション] セクションは、1 日に 1 件の E メールを生成します。

![[!UICONTROL 1 日のダイジェスト] メール [!UICONTROL 所有するプロジェクトに関する情報]](assets/admin-fund-user-notifications-06.png)

![[!UICONTROL 1 日のダイジェスト] メール [!UICONTROL 必要なアクション]](assets/admin-fund-user-notifications-07.png)

「毎日」オプションを選択する以外に、電子メールを送信する時間を設定します。 何が最適かに応じて、ダイジェストメールは、午前中に出社する前や当日出社直前に送信される場合があります。

![[!UICONTROL 1 日のダイジェストの電子メール送信後] ドロップダウンメニュー [!UICONTROL 担当者の編集] window](assets/admin-fund-user-notifications-08.png)

**まったく**

最後のオプションは、電子メール通知を完全に無効にすることです。

![選択した通知がオフになっています [!UICONTROL 担当者の編集] window](assets/admin-fund-user-notifications-09.png)

これを行う場合は、メールを受信していないにもかかわらず、内で作業の割り当て、コメント、更新が行われていることを知ってください [!DNL Workfront]. すべての通知をオフにすると、注意が必要な重要な情報が欠落している可能性があります。

以下の場合、 [!DNL Workfront] は、ユーザーが電子メール通知を無効にするのを確認しました。 例えば、ほとんどの作業を [!DNL Workfront] モバイルアプリでは、電子メール通知をオフにし、アプリからのみ通知を受け取ることができます。

に関係なく [!UICONTROL イベント通知] 通知を受け取ることにした場合、組織の目標に応じておこなわれる作業を成功させるには、通知が重要です。


## Recommendations

次のような通知が 2 つあります。 [!DNL Workfront] は、即時電子メールか 1 日のダイジェストかに関わらず、チェックをオンのままにすることをお勧めします。

ほとんどのユーザーに対して、次の操作を実行します。

* [!UICONTROL 担当タスクの先行タスクが完了した]
* [!UICONTROL 自分が更新を受信する対象者として追加された]
* [!UICONTROL 誰かが自分の作業項目にコメントを投稿しました]
* [!UICONTROL 自分に割り当てられているタスクの完了予定日が変更した]


特に、プロジェクトマネージャー向け：

* [!UICONTROL 自分が参加するプロジェクトの状況がアクティブになった]
* [!UICONTROL 自分が所有するプロジェクトに遅延が発生した]
* [!UICONTROL 自分が所有するプロジェクトに問題が追加された]
* [!UICONTROL マイルストーンタスクが自分のプロジェクトで完了しました]


<!---
learn more URLs
Email notifications
guide: manage your notifications
--->
