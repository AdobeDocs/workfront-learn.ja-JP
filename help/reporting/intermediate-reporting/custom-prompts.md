---
title: カスタムプロンプトの作成
description: カスタムプロンプトの概要、テキストモードを使用したカスタムプロンプトの作成方法、および Workfront でのレポートで使用できる例について説明します。
activity: use
feature: Text Mode Reporting
thumbnail: 336822.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-9087
exl-id: 1bb0832e-e888-4154-b78d-24c6d69f629f
doc-type: video
source-git-commit: 88c2161e897f23587ccc1d0e867b6f8961927a0f
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 98%

---

# カスタムプロンプトの作成

このビデオでは、次のことを学習します。

* カスタムプロンプトの概要
* テキストモードを使用したカスタムプロンプトの作成方法
* レポートで使用できる例

>[!VIDEO](https://video.tv.adobe.com/v/336822/?quality=12&learn=on)

## カスタムプロンプトアクティビティの作成

このページの PDF をダウンロードするには、[こちらをクリック](/help/assets/create-custom-prompts-activities.pdf)してください。

## アクティビティ：カスタムプロンプトの作成

1. プロンプトのドロップダウンメニューで次のプロジェクトステータスを表示するカスタムプロンプトを作成します。
   * 計画
   * 現在
   * 完了
   * 停止
1. プロンプトを変更して、今月が期限の現行プロジェクトを表示します。

## 解答

1. カスタムプロンプトは次のように表示され、次のテキストモードになります。

   ![テキストモードで新しいフィルターを作成する画面の画像](assets/cp-01.png)

   カスタムプロンプトを保存すると、プロンプトのドロップダウンメニューは次のように表示されます。

1. カスタムプロンプトのテキストモードは次のように表示されます。

![テキストモードで新しいフィルターを作成する画面の画像](assets/cp-02.png)

```
   status=CUR&plannedCompletionDate=$$TODAYbm&plannedCompletionDate_Mod=between&plannedCompletionDate_Range=$$TODAYem 
```

また、次のようなコードの変更を反映するように、アクティブなプロンプトのドロップダウンラベルを更新する必要があります。

![テキストモードで新しいフィルターを作成する画面の画像](assets/cp-02a.png)
