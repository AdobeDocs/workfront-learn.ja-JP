---
title: システム全体の問題ステータスのカスタマイズ
description: 問題のステータス名を変更する方法、ステータスが使用される問題のタイプを制御する方法、およびグループレベルのカスタマイズのロック/ロック解除のステータスを設定する方法について説明します。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
kt: 10030
exl-id: c8f5677f-8d9d-4d1a-a1e3-d1a438878213
source-git-commit: 02bc5a09a838be6d98c9b746bff731236ee4116f
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# システム全体のステータスのカスタマイズ

[!DNL Workfront] には、組織の問題管理ワークフローに対応するための様々なデフォルトの像が用意されています。 これらのステータスは、組織の用語に合わせて名前を変更できます。 ステータスは、特定のイシュータイプに割り当てることができます。

必要に応じて、追加のステータスを作成できます。 システム管理者のみが、システム全体のステータスを作成できます。 また、システム管理者は、グループ管理者が編集できるステータスを制御します。

![[!UICONTROL 問題] タブ [!UICONTROL 像] ページ内 [!UICONTROL 設定]](assets/admin-fund-all-issue-statuses.png)

## 既存のステータスの変更

[!DNL Workfront] では、ステータスの最小数を推奨しています。 これにより、ユーザーにとって適切なステータスの選択が容易になり、維持するステータスのリストが短くなります。

既存のステータスを編集して、名前、割り当て先の問題のタイプ、関連する色などを変更できます。

![問題ステータスリスト： [!UICONTROL 編集] 強調表示されたオプション](assets/admin-fund-edit-issue-status.png)

1. クリック **[!UICONTROL 設定]** 内 **[!UICONTROL メインメニュー]**.
1. を展開します。 **[!UICONTROL プロジェクト環境設定]** 」セクションを使用して、
1. 選択 **[!UICONTROL ステータス]**.
1. を選択します。 **[!UICONTROL 問題]** タブで、 [!UICONTROL システムステータス] が右上隅に表示されます。
1. 選択 **[!UICONTROL マスターリスト]** をクリックして、すべてのイシュータイプのステータスを確認します。 ここで、イシューステータスを作成または変更します。
1. 名前を変更するステータスの右側にマウスポインターを置いて、「 **[!UICONTROL 編集]**.
1. ステータスに新しい名前を付けるか、必要に応じて他の情報を変更します。
1. これらの設定を [!DNL Workfront] インスタンス。
1. ステータスのロックを解除して、グループ管理者が自分のグループのステータスのみを編集できるようにします。
1. ステータスを適用する問題のタイプのチェックボックスをオンにします。
1. クリック **[!UICONTROL 保存]**.

![新しいステータスを作成するためのウィンドウ](assets/admin-fund-edit-issue-status-2.png)

### ステータスの割り当て

すべてのステータスをすべてのイシュータイプに割り当てることはできません。 この [!UICONTROL ステータス] ページには、各ステータスを使用できる問題のタイプを示す列があります。

![ステータスページの「問題」タブでハイライト表示されている変更管理](assets/admin-fund-issue-type-statuses.png)


特定のイシュータイプに割り当てられたステータスのみを表示するには、ウィンドウ上部のイシュータイプ名をクリックします。

![[!UICONTROL 問題] タブ [!UICONTROL ステータス] 列が強調表示されたページ](assets/admin-fund-statuses-issue-type.png)

ここから、問題をドラッグ&amp;ドロップして、 [!UICONTROL ステータス] ドロップダウンメニュー。

ステータスを編集するには、次の場所に戻る必要があります： [!UICONTROL マスターリスト].
