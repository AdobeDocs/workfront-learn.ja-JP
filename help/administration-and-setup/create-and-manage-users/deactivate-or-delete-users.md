---
title: ユーザーをディアクティベートまたは削除するタイミングと方法
description: ユーザーをディアクティベートすることと削除することの違いについて説明します。 その後、組織のニーズに応じてユーザープロファイルを管理します。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner
thumbnail: 10037.jpeg
jira: KT-10037
exl-id: 89b7d083-97d3-4783-a61d-35226d6582c0
TQID: https://experienceleague.adobe.com/bOJ2ng-HrOD5SA9-uAItNK1rFF90zSnuxjeSiyh9LXk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 281
ht-degree: 87%

---

# ユーザーをディアクティベートまたは削除するタイミングと方法

ユーザーが組織を離れたときまたは [!DNL Workfront] を使用しなくなったときは、そのユーザーのログインをディアクティベートします。 ユーザープロファイルの削除は、特定の状況でのみ行う必要があります。

## ディアクティベート

ユーザーをディアクティベートすると、ユーザーのプロファイルからライセンスが削除されるので、ログインできなくなり、[!DNL Workfront] にもアクセスできなくなります。 そのユーザーのライセンスは、別のユーザーに割り当てて使用できます。

ディアクティベートされたユーザーに新しい作業を割り当てることはできませんが、既存の作業の割り当ては維持されます。

例えば、フリーランサーの作業が特定のプロジェクトに対して完了していて、次に必要になるまでログインを無効にしたい場合です。

## 削除

まれに、誤ったエントリーやテストユーザーなど、[!DNL Workfront] からユーザーログインを削除する必要が生じる場合があります。 ユーザーを削除すると、そのユーザーと [!DNL Workfront] 内の項目（作業の割り当て、メモ、時間、ドキュメント、作成したオブジェクトなど）との関連付けが削除されます

[!DNL Workfront] では、ユーザーの削除は、ユーザーが作業に割り当てられたことがない場合、または Workfront 項目との履歴がまったくない場合&#x200B;**のみ**&#x200B;に行うことをお勧めします。

[!DNL Workfront] では、ユーザーを削除する代わりに、ユーザーをディアクティベートすることを&#x200B;**強く**&#x200B;お勧めします。 非アクティブ化すると、[!DNL Workfront]にユーザー情報が保持されます。これは、正確なレポートやプロジェクト管理などに必要になる可能性があります。ユーザーを非アクティブ化するか削除するかについて質問がある場合は、[!DNL Workfront] コンサルタントまたは[!DNL Workfront] カスタマーサポートにお問い合わせください。

![[!DNL Users] ページでオプションを表示するその他メニュー](assets/admin-fund-adding-users-11.png)

### ユーザーをディアクティベートまたは削除する

1. [!UICONTROL メインメニュー]から、**[!UICONTROL ユーザー]**&#x200B;を選択します。
1. ユーザー名の横にあるボックスをオンにして、ユーザーを選択します。
1. **[!UICONTROL その他]**&#x200B;ドロップダウンメニューをクリックします。
1. 「**[!UICONTROL ディアクティベート]**」または「**[!UICONTROL 削除]**」を選択します。
