---
title: リスクありプルーフ設定のデフォルトの指定
description: プルーフ設定の一部として、危険プルーフ通知のデフォルト設定を指定する方法について説明します。
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: set-default-at-risk-proof-settings.png
jira: KT-10234
exl-id: 1e99e434-9aa5-44e3-8496-76dd57bd2f91
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: b18b693b-6d59-4359-95fd-a386b7a615fe
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T20:04:44.869Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 291
ht-degree: 100%

---

# リスクありプルーフ設定のデフォルトの指定

[!DNL Workfront] が送信する危険通知の設定を確立する必要があります。 これらは、まだ決定を行っていないプルーフの所有者と承認者に対し、念のため今後のプルーフの期限を知らせるリマインダーです。

危険通知はデフォルトでオンになっており、プルーフの期限の 24 時間前になるとプルーフは「危険」と見なされます。 [!DNL Workfront] では、この通知を 24 時間の時間枠でオンにしておくことをお勧めします。 ただし、組織でのプルーフターンアラウンド時間が数日ではなく数時間である場合は、この設定を数時間まで短縮することをお勧めします。

![危険通知のプルーフ設定](assets/proof-system-setups-at-risk-default-1.png)

1. [!DNL Workfront’s] の [!UICONTROL メインメニュー]から「**[!UICONTROL プルーフ]**」を選択します。
1. 上部のナビゲーションバーで「**[!UICONTROL アカウント設定]**」を選択します。
1. 「**[!UICONTROL 設定]**」タブを選択します。
1. 「[!UICONTROL プルーフのデフォルト]」セクションに移動します。
1. 「[!UICONTROL 危険な時間]」フィールドで、「**[!UICONTROL 設定]**」を選択します。 次に、プルーフの期限の何時間前に通知を送信するかを選択します。
1. その設定の「**[!UICONTROL 保存]**」を選択します。
1. 「[!UICONTROL 危険通知]」フィールドで[!UICONTROL 有効]と表示されていることを確認します。 表示されていない場合は、リンクをクリックして設定をオンにします。

## やってみよう

1. Workfront にログインし、設定エリアに移動します。 「レビューと承認」セクションで、指定したプルーフの受信者と非受信者に対する設定を選択します。
1. Workfront のメインメニューを使用して、プルーフの設定に移動します（「プルーフ」を選択）。 国、言語、タイムゾーンを、すべてのプルーフおよびプルーフユーザーのデフォルトに設定します。
1. 必要に応じて、プルーフ設定エリアの「設定」タブでリスクにある通知時間を調整します。 プルーフを使用してチームと話し合い、チームにとって何が最適かを判断します。

<!--
Lean More URLs
-->
