---
title: のグループとユーザー [!UICONTROL Workfront DAM]
description: でフォルダー、グループ、ユーザーを作成する方法を説明します。 [!UICONTROL Workfront DAM]. ユーザーの役割の種類を理解し、フォルダーに権限を付与します。
activity: use
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
team: Technical Marketing
kt: 8967
exl-id: 4ebf675c-b72d-447e-b131-a89acb449e15
source-git-commit: a0aa8328842d2db1235edc42664eb0b18f4038e4
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# システム設定：グループとユーザー

このビデオでは、次の方法を学習します。

* グループ設定がアセットへのアクセスに与える影響について
* 特定の順序でフォルダ、グループ、ユーザーを作成する
* ユーザーの役割のタイプについて
* フォルダーへの権限の付与
* グループの作成と編集
* ユーザーの追加と編集

>[!VIDEO](https://video.tv.adobe.com/v/335230/?quality=12)

## グループとユーザーのレビュー

設定時に [!UICONTROL Workfront DAM] システムの場合、大まかに見て、ユーザーやグループが果たす役割を考慮することが重要です。

グループは、内のアセットフォルダーへのアクセスを制御します。 [!UICONTROL Workfront DAM]. グループ設定では、ユーザーがアセット（表示、ダウンロード、編集など）を使用して実行できる操作も制御できます アクセス権があります。

グループを作成する際は、そのグループのメンバーがアクセスする必要があるアセットフォルダーを念頭に置いておくことが重要です [!UICONTROL Workfront DAM].

ユーザーは、 [!UICONTROL Workfront DAM]. ユーザーは、 [!UICONTROL Workfront DAM] グループに割り当てられていない場合に限ります。 ユーザーは、ニーズに応じて、複数のグループに属することができます。

## デフォルトのグループ

次の 2 つのデフォルトグループが用意されています： [!UICONTROL Workfront DAM]. すべてのユーザーは、 [!UICONTROL Workfront DAM] ログイン資格情報。 以下のグループに対してユーザーの追加や削除はできません。

* **ゲストグループ** — 匿名ユーザーのアクセスを制御するために使用します。 ログイン資格情報を持たないユーザーや、現在ログインしていないユーザーの場合があります。
* **ログ済み** — グループ内 — ログインしているすべてのユーザーがこのグループに属しています。

管理者グループとその設定も、デフォルトで存在します。 このグループにユーザを追加することはできますが、設定を調整することはできません。

## ロールのタイプ

グループが作成されると、ロールタイプが割り当てられます。 役割のタイプによって、 [!UICONTROL Workfront DAM] システムユーザーがログインすると、— [!UICONTROL Workfront DAM] 自身または [!UICONTROL Brand Connect].

で使用できる役割のタイプは 3 つあります。 [!UICONTROL Workfront DAM] ライセンス：

* **[!UICONTROL Brand Portal]** — これらのユーザーは、 [!UICONTROL Brand Connect]：ユーザーが承認済みアセットを表示およびダウンロードできる場所です。
* **[!UICONTROL 寄稿者]** — ユーザーが [!UICONTROL Workfront DAM] および [!UICONTROL Brand Connect]. アセットおよびフォルダーに対するフルアクセス権（表示、ダウンロード、アップロード、編集、移動、削除）を持ちます。
* **[!UICONTROL 管理者]** — システム管理者は、 [!UICONTROL Brand Connect] および [!UICONTROL Workfront DAM]に加えて、それぞれのグローバルシステム設定を確立する機能。 また、期限切れになった、または非アクティブに設定されたアセットにアクセスすることもできます。

<!-- 
Learn more graphic & documentation article link, below
* Understanding the difference between Workfront licenses and Workfront DAM role types
* -->
