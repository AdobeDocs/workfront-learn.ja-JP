---
title: 金融アクセスの理解
description: 金融アクセス権を使用して、管理者がWorkfrontで追跡される財務情報の表示と編集を行えるユーザーを制御する方法を説明します。
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-financial-access.png
type: Tutorial
role: User
level: Intermediate
kt: 10067
exl-id: 1c3d724a-8ff0-466f-9416-cff3da59c8ea
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 5%

---

# 金融アクセスの理解

組織が [!DNL Workfront]システム管理者は、その情報を表示および編集するためのアクセス権を持つユーザーを保護および管理する必要があります。

ユーザーが財務情報を表示または編集するには、次の 2 つが必要です。

1. アクセス権は [!UICONTROL アクセスレベル].
2. これらのアクセス権を使用する権限は、オブジェクト単位で付与する必要があります。

例えば、ユーザーには、財務データをアクセスレベルで表示する権限を付与できますが、そのユーザーと共有され、そのタスクの共有時に財務データを表示できるのは、タスクの財務データのみです。

したがって、 [!UICONTROL アクセスレベル] オブジェクトの個々の共有オプションに応じて、一部のオブジェクトで金融を表示し、他のオブジェクトでは金融を表示する権利。 ただし、ユーザーがオブジェクトで財務を表示できるのは、そのユーザーに権限が与えられている場合を除きます [!UICONTROL アクセスレベル].

## [!UICONTROL アクセスレベル] 設定

金融データへの全体的なアクセス権は、次の方法で最初に付与されます： [!DNL Workfront] ライセンスの種類。

**[!UICONTROL プラン] ライセンスには次のことができます。**

* 請求レコードの管理
* 役割の請求とコスト率を管理および表示します
* ユーザーの請求とコスト率の管理と表示
* 費用の管理
* 財務の表示と編集

**[!UICONTROL 作業] ライセンスには次のことができます。**

* 費用の管理
* 財務の表示

**[!UICONTROL レビュー] ライセンスには次のことができます。**

* 財務の表示

**権限は [!UICONTROL アクセスレベル]. 金融データアクセスには、次の 3 つのオプションがあります。**

* [!UICONTROL アクセスなし]  — ユーザーは財務情報を見ることができません。
* [!UICONTROL 表示]  — ユーザーは、情報を確認し、共有できます。
* [!UICONTROL 編集]  — ユーザーは、情報を作成、編集、削除、共有できます。 （プランライセンスでのみ利用可能）

![一般的な財務データオプションをアクセスレベルで示す画像](assets/setting-up-finances-8.png)

重要なのは [!UICONTROL 表示] および [!UICONTROL 編集] オプションには、 [!UICONTROL プラン] ライセンス。 の歯車をクリックします。 [!UICONTROL 表示] ボタンを使用して、次のオプションを設定できます。

**[!UICONTROL ビュー]**

* 役割請求率と役割コスト率を表示
* ユーザー請求率とユーザーコスト率を表示

![アクセス・レベルでの財務データ・ビュー・オプションを示す画像](assets/setting-up-finances-9.png)

**[!UICONTROL 編集]**

これら 2 つのオプションは、 [!UICONTROL 編集] オプションと次の情報：

* 役割請求率と役割コスト率を編集
* ユーザー請求率とユーザー コスト率を編集

![アクセスレベルでの財務データ編集オプションを示す画像](assets/setting-up-finances-10.png)

>[!NOTE]
>
>費用を追加するアクセス権を持つユーザーは、追加した費用と、直属の部下が追加した費用も表示できます。
