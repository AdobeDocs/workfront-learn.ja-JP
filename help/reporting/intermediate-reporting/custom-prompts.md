---
title: カスタムプロンプトの作成
description: カスタムプロンプトの概要、テキストモードを使用したカスタムプロンプトの作成方法、およびWorkfrontでのレポートで使用できる例を説明します。
activity: use
feature: Reports and Dashboards
thumbnail: 336822.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9087
exl-id: 1bb0832e-e888-4154-b78d-24c6d69f629f
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 2%

---

# カスタムプロンプトの作成

このビデオでは、次のことを学習します。

* カスタムプロンプトとは
* テキストモードを使用してカスタムプロンプトを作成する方法
* レポートで使用できる例

>[!VIDEO](https://video.tv.adobe.com/v/336822/?quality=12)

## アクティビティ：カスタムプロンプトの作成

1. プロンプトのドロップダウンメニューに次のプロジェクトステータスを表示するカスタムプロンプトを作成します。
   * 計画
   * 現在
   * 完了
   * 停止
1. プロンプトを変更して、今月期限の現在のプロジェクトを表示します。

## 回答

1. カスタムプロンプトは次のようになり、次のテキストモードになります。

   ![テキストモードで新しいフィルターを作成するための画面の画像](assets/cp-01.png)

   カスタムプロンプトを保存すると、プロンプトのドロップダウンメニューは次のようになります。

1. カスタムプロンプトのテキストモードは次のようになります。

![テキストモードで新しいフィルターを作成するための画面の画像](assets/cp-02.png)

```
   status=CUR&plannedCompletionDate=$$TODAYbm&plannedCompletionDate_Mod=between&plannedCompletionDate_Range=$$TODAYem 
```

また、次のようなコードの変更を反映するように、アクティブなプロンプトのドロップダウンラベルを更新する必要があります。

![テキストモードで新しいフィルターを作成するための画面の画像](assets/cp-02a.png)
