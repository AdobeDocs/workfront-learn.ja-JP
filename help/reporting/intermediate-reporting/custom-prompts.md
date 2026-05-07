---
title: テキストモードを使用したカスタムプロンプトの作成
description: カスタムプロンプトの概要、テキストモードを使用したカスタムプロンプトの作成方法、および Workfront でのレポートで使用できる例について説明します。
activity: use
feature: Reports and Dashboards
thumbnail: 336822.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: '2025-08-05T00:00:00.000Z'
jira: KT-9087
exl-id: 1bb0832e-e888-4154-b78d-24c6d69f629f
doc-type: video
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: c6dd2ac5-f5bd-4e59-9101-25b156918623
subfeature_v2: id: cec4c78b-dd2b-46ec-b824-6ca30f0eb7b2
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-06T13:58:55.263Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 207
ht-degree: 94%

---

# テキストモードを使用したカスタムプロンプトの作成

このビデオでは、次のことを学習します。

* カスタムプロンプトの概要
* テキストモードを使用したカスタムプロンプトの作成方法
* レポートで使用できる例

>[!VIDEO](https://video.tv.adobe.com/v/336822/?quality=12&learn=on&enablevpops=0)

## 「カスタムプロンプトの作成」アクティビティ


### アクティビティ：カスタムプロンプトの作成

1. プロンプトのドロップダウンメニューで次のプロジェクトステータスを表示するカスタムプロンプトを作成します。
   * 計画
   * 現在
   * 完了
   * 停止
1. プロンプトを変更して、今月が期限の現行プロジェクトを表示します。

### 解答

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
