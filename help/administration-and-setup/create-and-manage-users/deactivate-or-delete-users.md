---
title: ユーザーを非アクティブ化または削除するタイミングと方法
description: ユーザーの非アクティブ化と削除の違いについて説明します。 その後、組織のニーズに応じてユーザープロファイルを管理します。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner
thumbnail: 10037.jpeg
kt: 10037
exl-id: 89b7d083-97d3-4783-a61d-35226d6582c0
source-git-commit: adf12d7846d2a1b4c32513a3955c080905044576
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---

# ユーザーを非アクティブ化または削除するタイミングと方法

ユーザーが組織を離れたとき、または使用しなくなったとき [!DNL Workfront]に設定されている場合、ログインを非アクティブ化します。 ユーザープロファイルの削除は、特定の状況でのみおこなう必要があります。

## 非アクティブ化

ユーザーを非アクティブ化すると、ユーザーのプロファイルからライセンスが削除されるので、ログインできなくなったり、にアクセスできなくなります [!DNL Workfront]. ライセンスを使用して別のユーザーに割り当てることができます。

非アクティブなユーザーは、新しい作業を割り当てることはできませんが、既存の作業に割り当てられたままになります。

例えば、フリーランサーの作業が特定のプロジェクトに対して完了している場合、次に必要になるまでログインを無効にしたいと考えます。

## 削除

まれに、誤ったエントリやテストユーザーなど、ユーザーログインを削除する必要が生じる場合があります。 [!DNL Workfront]. ユーザーを削除すると、そのユーザーと内の項目との関連付けが削除されます [!DNL Workfront] — 作業の割り当て、メモ、時間、ドキュメント、作成したオブジェクトなど

この **のみ** 時間 [!DNL Workfront] ユーザーの削除は、ユーザーがまだ作業に割り当てられていない場合、またはWorkfront項目の履歴がまったくない場合におこなうことをお勧めします。

[!DNL Workfront] **強く** では、ユーザーを削除する代わりに、ユーザーを非アクティブ化することをお勧めします。 非アクティブ化すると、のユーザー情報が保持されます。 [!DNL Workfront]（正確なレポート、プロジェクト管理などに必要になる場合があります） ユーザーのアクティベートを解除するか削除するかについて質問がある場合は、 [!DNL Workfront] コンサルタントまたは [!DNL Workfront] カスタマーサポート。

![オプションを表示する [ その他 ] メニュー [!DNL Users] ページ](assets/admin-fund-adding-users-11.png)

### ユーザーの非アクティブ化または削除

1. 選択 **[!UICONTROL ユーザー]** から [!UICONTROL メインメニュー].
1. ユーザー名の横にあるボックスをオンにして、ユーザーを選択します。
1. 次をクリック： **[!UICONTROL 詳細]** ドロップダウンメニュー。
1. 選択 **[!UICONTROL 無効化]** または **[!UICONTROL 削除]**.
