---
title: グローバルおよび単一使用の承認プロセスの作成
description: Workfront のプロジェクト、タスク、イシューで単一使用承認プロセスを作成する方法を説明します。
activity: use
feature: Approvals
thumbnail: 335225.jpeg
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-8962
last-substantial-update: 2024-09-24T00:00:00Z
recommendations: noDisplay,noCatalog
exl-id: 85d28b54-72a6-4dd1-bac8-8e7ffb3e2b76
doc-type: video
source-git-commit: b0114985964736fb7bb234c581cb56930714915c
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 42%

---

# グローバルおよび単一使用の承認プロセスの作成

プロジェクト、タスク、イシューの承認プロセスを使用すると、プロジェクトマネージャーは、作業が完了したことを事前に専門家に確認してから、作業を進めることができます。プロジェクトマネージャーは、状況に応じて承認プロセスを作成したり（これは、1 回限りの承認プロセスと呼ばれます）、一般的なニーズを満たすために以前に作成された可能性のある多数の承認プロセスのリストから選択したり（これらを、グローバル承認プロセスや既存の承認プロセスと呼びます）できます。

どちらの場合も、オブジェクトのステータスが承認プロセスで指定されたステータスに変わると、承認者は作業をレビューして承認または拒否するように、様々な方法で通知されます。承認待ちの状態でプロジェクト全体が一時停止される場合があるので、承認者は、承認を求められる場合があることを事前に認識しておく必要があります。承認者が何らかの理由で不在の場合、適格な代替者に承認をデリゲートできます。詳しくは、[タスク、イシュー、承認のデリゲート](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)を参照してください。

このビデオでは、プロジェクト、タスクまたはイシューに対して、グローバル承認プロセスと単一使用の承認プロセスを作成する方法について説明します。

>[!VIDEO](https://video.tv.adobe.com/v/335225/?quality=12&learn=on)

>[!TIP]
>
>プロジェクトまたはタスクに対して単一使用承認プロセスをプロジェクトテンプレートに追加できます。

>[!NOTE]
>
>ビデオのタスクについて説明したのと同じ方法で、プロジェクトとイシューに対して単一使用の承認を設定できます。

## リクエストキューでイシューの自動承認を適用する方法

リクエストキューで自動問題承認を設定する場合は、グローバル問題承認プロセスのみを使用して設定でき、[!UICONTROL  キュートピック ] に適用されます。

[!UICONTROL  キュートピック ] を作成または編集する際に、「**[!UICONTROL デフォルトの承認]**」フィールドでグローバル承認プロセスを選択します。

![ キュートピックでデフォルトの承認プロセスを選択する方法を示す画像 ](assets/automatic-issue-approval-1.png)

イシューの承認プロセスを編集して、承認が拒否されたときに **[!UICONTROL 前のステータス]** がイシューが設定されたものではないことを確認する必要がある場合があります。 これは、前のステータスが **[!UICONTROL 新規]** で、これは承認プロセスをトリガーするステータスでもあるので、承認時に設定されるステータスであるためです。 問題の承認が却下された場合の混乱を避けるために、ステータスを **[!UICONTROL 解決しない]** や、この目的で作成されたカスタムステータスなどに設定することをお勧めします。

![ イシューが拒否されたときに使用するステータスの変更を示す画像 ](assets/automatic-issue-approval-2.png)


## このトピックに関する推奨チュートリアル

* [タスク、イシュー、承認を委任する](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)
* [既存の承認プロセスの添付と編集](/help/manage-work/approval-processes-and-milestone-paths/attach-and-edit-existing-approval-processes.md)
* [グループ特有の承認プロセスについて](/help/administration-and-setup/approval-processes-and-milestone-paths/group-specific-approval-processes.md)
* [リクエストフローの作成](/help/manage-work/request-queues/create-a-request-flow.md)

