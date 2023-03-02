---
title: 基本的な条件付き書式の追加
description: 列ルールを使用して、設定した条件に基づいて、レポートまたはビューのテキストの色、書式、背景色を変更する方法を説明します。
activity: use
feature: Reports and Dashboards
thumbnail: 335149.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8855
exl-id: bf9a4cf4-b073-4f7e-8516-e7843f4dc20f
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# ビューへの基本的な条件付き書式の追加

条件付き書式は、列ルールを作成しておこないます。 列ルールを使用すると、設定した条件に基づいて、特定の形式で列を書式設定できます。

このビデオでは、次のことを学習します。

* ビューに表示される条件付き書式
* 条件付き書式の作成および変更方法

>[!VIDEO](https://video.tv.adobe.com/v/335149/?quality=12)

## アクティビティ：ビューへの条件付き書式の追加

既存の標準ビューを使用し、この条件付き書式を [!UICONTROL 名前] 列。

1. タスクの進捗状況の状態が [ 遅延 ] の場合に、フィールドの背景を赤に変える段間罫線を追加します。
1. 進捗状況のステータスが [ 背後 ] または [ 危険 ] の場合に、フィールドの背景を黄色に変える列ルールを追加します。

これにより、進行状況の列をビューの一部に含めずに、問題のあるタスクを見つけるのに役立ちます。

## 回答

![新しい列ルールを作成する画面の画像](assets/conditional-formatting-exercise.png)

1. タスクリストレポートで、 **[!UICONTROL 表示]** ドロップダウンメニューで「 」を選択します。 **[!UICONTROL 新しいビュー]**.
1. ビューに「Standard + Progress」と名前を付けます。
1. 指定されたデフォルトの列を使用します。
1. を選択します。 [!UICONTROL タスク名] 列。 これは、条件付き書式を適用する列です。タスクの進捗状況の状態が [ オンタイム ] でない場合は、赤または黄色で表示されます。
1. クリック **[!UICONTROL 詳細オプション]** をクリックします。
1. クリック **[!UICONTROL この列にルールを追加]**.
1. 次を変更して列ルールを開始 [!UICONTROL タスク] > [!UICONTROL 名前] 窓の上に [!UICONTROL タスク] > [!UICONTROL 進捗状況ステータス]. クリックするだけで **[!UICONTROL X]** 隣のアイコン [!UICONTROL タスク] > [!UICONTROL 名前] をクリックして、フィールドから削除します。
1. フィールドに「進行状況」を入力し、「 」を選択します。 [!UICONTROL 進捗状況ステータス] の下に [!UICONTROL タスク] フィールドソース。
1. 選択 **[!UICONTROL 遅延]** の右側のフィールド内 [!UICONTROL 次と等しい] 修飾子。
1. 赤の背景を [!UICONTROL テキストカラー] 行
1. クリック **[!UICONTROL ルールを追加]** 」と入力して、段間罫線を保存します。
1. 今すぐクリック **[!UICONTROL 段間罫線を追加]** 別のルールを追加する場合にもう一度使用します。
1. 前と同様に、削除します [!UICONTROL タスク] > [!UICONTROL 名前] を「条件」フィールドから選択します。 次で置き換えます。 [!UICONTROL 進捗状況ステータス] の下に [!UICONTROL タスク] フィールドソース。
1. 両方を選択 [!UICONTROL リスク] および [!UICONTROL 後ろ] が Equal 修飾子の右側のフィールドに含まれています。
1. で黄色の背景を選択します。 [!UICONTROL テキストカラー] 行
1. クリック **[!UICONTROL ルールを追加]** 」と入力して、段間罫線を保存します。
1. クリック **[!UICONTROL ビューを保存]** をクリックしてビューを保存します。
