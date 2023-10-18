---
title: グループとユーザーの設定
description: '[!UICONTROL Workfront DAM] でフォルダー、グループ、ユーザーを作成する方法を説明します。ユーザーの役割タイプを理解し、フォルダーに権限を付与します。'
activity: use
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
team: Technical Marketing
jira: KT-8967
exl-id: 4ebf675c-b72d-447e-b131-a89acb449e15
doc-type: video
source-git-commit: 6c31f8d2e98ad8cd1880cd03ec0b0e6c0fd9ec09
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 88%

---

# グループとユーザーの設定

このビデオでは、以下の方法を説明します。

* グループ設定がアセットへのアクセス権に与える影響について
* 特定の順序でのフォルダー、グループ、ユーザーの作成
* ユーザーの役割タイプの理解
* フォルダーへの権限の付与
* グループの作成と編集
* ユーザーの追加と編集

>[!VIDEO](https://video.tv.adobe.com/v/335230/?quality=12&learn=on)

## グループとユーザーのレビュー

設定時に、 [!UICONTROL Workfront DAM] システムの場合、大まかに見て、ユーザーやグループが果たす役割を考慮することが重要です。

グループは、[!UICONTROL Workfront DAM] のアセットフォルダーへのアクセスを制御します。また、グループ設定は、ユーザーがアクセス権を持つアセットに対して実行できる操作（表示、ダウンロード、編集など）も制御します。

グループを作成する際は、そのグループのメンバーがアクセスする必要があるアセットフォルダーを念頭に置いておくことが重要です [!UICONTROL Workfront DAM].

ユーザーは、[!UICONTROL Workfront DAM] にログインしている個人です。ユーザーは、グループに割り当てられていない限り、[!UICONTROL Workfront DAM] のいずれにもアクセスできません。ユーザーは、必要に応じて複数のグループに属することができます。

## デフォルトのグループ

[!UICONTROL Workfront DAM] には 2 つのデフォルトのグループがあります。すべてのユーザーは、[!UICONTROL Workfront DAM] ログイン資格情報を持っているかどうかに基づいて、これらのグループに自動的に属します。以下のグループからユーザーを追加または削除することはできません。

* **ゲストグループ** - 匿名ユーザーのアクセスを制御するために使用します。これは、ログイン資格情報を持たないユーザーや、現在ログインしていないユーザーである可能性があります。
* **ログ**&#x200B;イングループ - ログインしているすべてのユーザーがこのグループに属します。

管理者グループとその設定もデフォルトで存在します。このグループにユーザーを追加することはできますが、設定を調整することはできません。

## 役割タイプ

グループを作成すると、役割タイプが割り当てられます。役割タイプは、[!UICONTROL Workfront DAM] システムユーザーが [!UICONTROL Workfront DAM] 自体または [!UICONTROL Brand Connect] にログインした際に取得する部分を決定します。

[!UICONTROL Workfront DAM] ライセンスで使用できる役割タイプは 3 つあります。

* **[!UICONTROL Brand Portal]** - これらのユーザーは、承認済みアセットを表示およびダウンロードできる [!UICONTROL Brand Connect] にのみアクセスできます。
* **[!UICONTROL 投稿者]** - これらのユーザーは、[!UICONTROL Workfront DAM] および [!UICONTROL Brand Connect] にアクセスできます。アセットとフォルダーへの完全なアクセス権（表示、ダウンロード、アップロード、編集、移動、削除）を持っています。
* **[!UICONTROL 管理者]** - システム管理者は [!UICONTROL Brand Connect] と [!UICONTROL Workfront DAM] のすべてにアクセスできるほか、それぞれのグローバルシステムの設定を行うことができます。また、有効期限が切れているか、非アクティブに設定されているアセットにアクセスすることもできます。

<!-- 
Learn more graphic & documentation article link, below
* Understanding the difference between Workfront licenses and Workfront DAM role types
* -->
