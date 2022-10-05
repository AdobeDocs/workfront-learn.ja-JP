---
title: リソース管理ツールでの表示
description: 主な担当者とは何か、およびリソース管理に与える影響について説明します。
feature: Resource Management
type: Tutorial
role: Leader, User
level: Intermediate, Experienced
activity: use
team: Technical Marketing
kt: 10184
exl-id: 3818c7fb-b820-4002-bf49-9c79c9f0afb2
source-git-commit: 02bc5a09a838be6d98c9b746bff731236ee4116f
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 1%

---

# リソース管理ツールでの表示

リソースの計画と管理にとって、誰がいつ利用できるかを把握することが不可欠です。 ユーザーがWorkfrontのカレンダーで自分の休日をマークすると、その情報はWorkfrontのリソースツールでも確認できます。

## リソースプランナー

ユーザーのオフ時間は、リソースプランナーの「利用可能 (AVL) 」列に反映されます。 Workfrontは、割り当てられたスケジュール、ジョブロールの割合などに基づいてWorkfrontが計算する、使用可能な時間からカレンダーにマークされたオフ時間を引きます。

![使用可能な列でのオフ時間](assets/vis_01.png)

## ワークロードバランサー

ワークロード・バランサでは、タイムオフはカレンダに灰色のバーで表示されます。 この表示設定により、リソースマネージャや他のユーザーが作業を割り当てる際に、より十分な情報に基づいた意思決定を行うことができます。

ただし、タイムオフインジケータは、ワークロードバランサーを通じてユーザーに作業を割り当てることを妨げません。 作業が割り当てられている場合、ワークロード・バランサは、その人物がオフ期間中に過剰に割り当てられていることを示します。

![灰色のバーの時間](assets/vis_02.png)
