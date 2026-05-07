---
title: 日付ベースのワイルドカードを使用したフィルターの作成
description: 日付ベースのワイルドカードを使用する方法とタイミング、および現在の日付に基づいてフィルターを作成する方法について説明します。
activity: use
feature: Reports and Dashboards
thumbnail: 336812.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: '2025-06-27T00:00:00.000Z'
jira: KT-9082
exl-id: 0f7db4eb-a062-4eb3-99ca-c40d8e266943
doc-type: video
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: c6dd2ac5-f5bd-4e59-9101-25b156918623
subfeature_v2: id: ceb4d94a-32ed-4fea-9724-1339d684b0bc
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-06T13:57:08.996Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 246
ht-degree: 100%

---

# 日付ベースのワイルドカードを使用したフィルターの作成

このビデオでは、以下の方法を説明します。

* 日付ベースのワイルドカードを使用するタイミングを理解する
* Workfront で使用する 2 つの日付ベースのワイルドカードの違いを理解する
* 日付ベースのワイルドカードをフィルターに追加する
* ワイルドカード、属性、演算子、修飾子を使用してカスタム日付を作成する
* ワイルドカードを使用してカスタムの日付範囲を作成する

>[!VIDEO](https://video.tv.adobe.com/v/336812/?quality=12&learn=on&enablevpops=0)


## 「日付ベースのワイルドカードを使用したフィルターの作成」アクティビティ


### アクティビティの設問

1. イシューの期限を昨日または今日に設定するとしたら、どのようにフィルタールールを作成しますか？
1. 期限が先週のプロジェクトを検索するとしたら、どのようにフィルタールールを作成しますか？
1. 次のフィルタルールは、定期的に使用するタスクレポートの一部です。 このレポートから得られるのは、どのようなタイプの結果ですか？

![日付ベースのワイルドカードを使用してタスクフィルターを作成する画面の画像](assets/date-wildcard-answer-1.png)

### 解答

1. イシューの予定完了日を [!UICONTROL $$TODAY-1d] と [!UICONTROL $$TODAY] の間でフィルタリングします。
1. プロジェクトの予定完了日を [!UICONTROL $$TODAYb-1w] と [!UICONTROL $$TODAYe-1w] の間でフィルタリングします。
1. このレポートは、自分に割り当てられていて、まだ完了していない（つまり、完了率が 100 未満である）、期限を過ぎているか期限が今日のタスクを検索します。 タスクの予定完了日のフィルタールールは、期限が本日以前のタスクを調べるという意味です。
