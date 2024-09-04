---
title: プロジェクトタイムラインからの進捗の追跡
description: ' [!DNL  Workfront]  で、完了率や、ステータス、割り当て、制約を使用して、プロジェクトタイムラインから進捗を追跡する方法を説明します。'
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: track-work-progress-from-the-project-timeline.jpeg
type: Tutorial
role: User
last-substantial-update: 2023-08-16T00:00:00Z
level: Beginner
jira: KT-10150
hide: true
source-git-commit: 609df4be7b1115b7b624d9e8e758845cd2a51bdb
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 100%

---

# プロジェクトタイムラインからの進捗の追跡

プロジェクトの期限に間に合うように、タスクが順調に進行していることを確認します。[!UICONTROL タスク]のリストにざっと目を通すと、[!DNL  Workfront] には作業の進捗やステータスを監視するのに役立つ機能がいくつかあります。

## 完了率

各作業タスクの完了率は、作業の進捗を測定するために使用される場合があります。このフィールドは担当者の予測によるものなので、手動で調整する必要があることに注意してください。

>[!TIP]
>
>作業タスクの完了率は手動で更新する必要がありますが、親タスクの完了率は、完了率と各子タスクの期間または予定時間数に基づいて、Workfront で計算されます。つまり、大きなタスクを小さなサブタスクに分割すると、完了率の精度が向上します。


![[!UICONTROL 完了率]の列が表示されているプロジェクトタスクリスト](assets/planner-fund-task-percent-complete.png)

完了率は次の 3 つの場合に自動で変更されます。

* タスクの[!UICONTROL ステータス]が「完了」に設定された場合は、完了率が 100 に変わります。
* タスクの[!UICONTROL ステータス]が「新規」にロールバックされた場合は、完了率が 0 にリセットされます。
* 親タスクで、子タスクの完了率が変更された場合。

## ステータス

[!UICONTROL ステータス]列を[!UICONTROL ビュー]に含めると、開始されたタスク、進行中のタスク、完了したタスクがどれかをすばやく確認できます。[!UICONTROL ビュー]で条件付き書式を設定して、各ステータスを色分けし、情報を判別しやすくすることもできます。

## タスクの割り当て

プロジェクトをレビューする際は、タスクの割り当てをレビューします。作業が遅れたのは、タスクに誰も割り当てられなかったことが原因かもしれません。あるいは、割り当てられたユーザーに、作業を完了するための適切なスキルセットがなかった場合。タスクに担当者を追加するか、タスクを再割り当てして、作業を確実に完了させます。

## タスクの制約

タスクの制約が変更され、ユーザーがそれに気付かないことがあります。制約はタイムラインの挙動に影響を与える可能性があるので、制約が意図通りに設定されていることを確認する必要があります。

![タスクの制約の列が表示されているプロジェクトのタスクのリスト](assets/planner-fund-task-constraint.png)

タスクのリストでこの情報を確認できるように、[!UICONTROL タスクの制約]列を含むカスタムビューを作成します。 開始日からプロジェクトを計画した場合は、タスクに「[!UICONTROL できるだけ早く]（[!UICONTROL ASAP]）」の制約を設定します。

タスクの制約について詳しくは、[期間のタイプとタスクの制約の理解と管理](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/intermediate-projects/understand-and-manage-duration-types-and-task-constraints.html?lang=ja)を参照してください。
