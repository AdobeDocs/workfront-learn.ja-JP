---
title: 基本フィルターアクティビティの作成
description: このビデオでは、Workfrontで独自のフィルターを作成するアクティビティを実行します。
activity: use
feature: Reports and Dashboards
thumbnail: 336807.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8856
exl-id: fc29b4ce-2937-478e-abd5-0b559657ead0
source-git-commit: b09d634a8b4ec32eda2663f1df04cc8bc04596a9
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 0%

---

# 基本フィルターアクティビティの作成

このビデオでは、「今月を閉じるプロジェクトを所有」という名前のプロジェクトフィルターを作成します。 多くのプロジェクトに目を向けている場合は、このフィルターを使用して、間もなく閉じる予定のプロジェクトを拡大できます。

詳細な手順については、以下を参照してください。

>[!VIDEO](https://video.tv.adobe.com/v/336807/?quality=12)

## 回答

![新しいフィルターを作成する画面の画像](assets/basic-filter-activity-updated-6-15-21.png)

1. 次に移動： [!UICONTROL プロジェクト] 領域 [!UICONTROL メインメニュー]. プロジェクトのリストが表示されます。
1. 次をクリック： **[!UICONTROL フィルター]** メニューと選択 **[!UICONTROL 新しいフィルター]**.
1. フィルターに「今月終了するプロジェクトを所有」という名前を付けます。
1. クリック **[!UICONTROL フィルタールールを追加]**.
1. 内 [!UICONTROL フィールド名の入力を開始] 「所有者」と入力します。 次に、 [!UICONTROL 所有者 ID] の下に [!UICONTROL プロジェクト] フィールドソース。
1. を [!UICONTROL 次と等しい] 演算子をそのまま使用します。
1. 「名前の入力を開始」フィールドに「$$」と入力します。
1. 選択 [!UICONTROL $$USER.ID]. これは、ログインしているユーザーのワイルドカードです。
1. クリック [!UICONTROL フィルタールールを追加] 再び
1. 内 [!UICONTROL フィールド名の入力を開始] フィールドに、「完了」と入力します。 次に、 [!UICONTROL 完了] をクリックします。
1. を [!UICONTROL 次と等しい] 演算子をそのまま使用します。
1. 「False」を選択します。
1. クリック [!UICONTROL フィルタールールを追加] 再び
1. 内 [!UICONTROL フィールド名の入力を開始] 「計画済み」フィールドタイプを選択し、「 [!UICONTROL 計画完了日] の下に [!UICONTROL プロジェクト] フィールドソース。
1. を [!UICONTROL 次と等しい] 演算子 [!UICONTROL 今月].
1. クリック **[!UICONTROL フィルターを保存]**
