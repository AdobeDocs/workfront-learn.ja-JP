---
title: 基本的なフィルターの作成アクティビティ
description: このアクティビティでは、「今月終了する自分のプロジェクト」という名前のプロジェクトフィルターを作成します。
activity: use
feature: Reports and Dashboards
thumbnail: 336807.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8856
exl-id: fc29b4ce-2937-478e-abd5-0b559657ead0
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: ht
source-wordcount: '231'
ht-degree: 100%

---

# 基本的なフィルターの作成アクティビティ

このビデオでは、「今月終了する自分のプロジェクト」という名前のプロジェクトフィルターを作成します。多くのプロジェクトを監視している場合は、このフィルターを使用すると、まもなく完了する予定のプロジェクトに注目するのに役立ちます。

詳細な手順の説明がページの後半にあります。

>[!VIDEO](https://video.tv.adobe.com/v/336807/?quality=12)

## 回答

![新しいフィルターを作成する画面の画像](assets/basic-filter-activity-updated-6-15-21.png)

1. [!UICONTROL メインメニュー]から[!UICONTROL プロジェクト]エリアに移動します。プロジェクトのリストが表示されます。
1. **[!UICONTROL フィルター]**&#x200B;メニューをクリックして、「**[!UICONTROL 新しいフィルター]**」を選択します。
1. フィルターに「今月終了する自分のプロジェクト」
という名前を付けます。
1. 「**[!UICONTROL フィルタールールを追加]**」をクリックします。
1. 「[!UICONTROL フィールド名の入力を開始]」フィールドで「所有者」と入力します。それから、「[!UICONTROL プロジェクト]」フィールドソースの下にある「[!UICONTROL 所有者 ID]」を選択します。
1. 「[!UICONTROL 次と等しい]」演算子はそのままにしておきます。
1. 「名前の入力を開始」フィールドに「$$」と入力します。
1. 「[!UICONTROL $$USER.ID]」を選択します。これは、ログイン中のユーザーに対するワイルドカードです。
1. もう一度「[!UICONTROL フィルタールールを追加]」をクリックします。
1. 「[!UICONTROL フィールド名の入力を開始]」フィールドで「完了」と入力します。それから、「プロジェクト」フィールドソースの下にある「[!UICONTROL 完了]」を選択します。
1. 「[!UICONTROL 次と等しい]」演算子はそのままにしておきます。
1. 「False」を選択します。
1. もう一度「[!UICONTROL フィルタールールを追加]」をクリックします。
1. 「[!UICONTROL フィールド名の入力を開始]」フィールドで「予定」と入力し、「[!UICONTROL プロジェクト]」フィールドソースの下にある「[!UICONTROL 予定完了日]」を選択します。
1. 「[!UICONTROL 次と等しい]」演算子を「[!UICONTROL 今月]」に変更します。
1. 「**[!UICONTROL フィルターを保存]**」をクリックします。
