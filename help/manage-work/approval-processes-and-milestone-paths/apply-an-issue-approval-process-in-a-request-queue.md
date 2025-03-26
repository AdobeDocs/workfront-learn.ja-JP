---
title: リクエストキューにイシュー承認プロセスを適用
description: デフォルトの承認プロセスを実装してリクエストワークフローを効率化し、承認されたリクエストのステータスが「新規」に適切に変更されるようにします。 「解決されません」へのステータス変更を選択することで、却下されたリクエストの混乱に対処します。
activity: use
feature: Approvals
thumbnail: 335225.jpeg
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-17578
last-substantial-update: 2025-03-26T00:00:00Z
recommendations: noDisplay,catalog
doc-type: video
source-git-commit: 3fc3a58c829769ca06ffb93971ac75516dfbd5f2
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 5%

---

# リクエストキューにイシュー承認プロセスを適用

>[!PREREQUISITES]
>
>* [リクエストフローの作成](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/create-a-request-flow)
>* [ グローバルおよび単一使用の承認プロセスの作成 ](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)


このビデオでは、リクエストキューの作成時にデフォルトの承認プロセスを適用するプロセスを説明します。&#x200B; リクエストが作成されると、ステータスが「新規 – 承認待ち」で開始し、指定された承認者に承認通知が送信されます。&#x200B; 承認されると、ステータスが「新規」に変わり、割り当てられた個人が作業を開始できるようになります。&#x200B; 拒否された場合、承認プロセスの設定でよくある間違いにより、ステータスが誤って「新規」に戻る場合があります。&#x200B;
このビデオでは、ステータスが「新規」（新しいリクエストのデフォルト）に設定されると、承認プロセスがトリガーされることをハイライト表示しています。&#x200B; 拒否された場合、システムはデフォルトでステータスを以前の状態に戻します。これは、新しいリクエストには理想的ではありません。&#x200B; 代わりに、「解決されない」などの別のステータスを選択する必要があります。&#x200B; また、このビデオでは、デフォルトで「却下」ステータスは提供されていないことにも注意しますが、システム管理者は必要に応じて作成できます。&#x200B;

>[!VIDEO](https://video.tv.adobe.com/v/3455013/?quality=12&learn=on&enablevpops)

## 重要ポイント

* **デフォルトの承認プロセス：** リクエストキューを作成する際に、各リクエストに承認ワークフローを自動的に割り当てるデフォルトの承認プロセスを適用できます。
* **承認時のステータス変更：** 承認されたリクエストのステータスは「新規 – 承認待ち」から「新規」に変更され、割り当てられた個人が作業を開始できるようになります。
* **拒否処理でよくある間違い：** リクエストが拒否されると、承認プロセスのデフォルトのシステム設定により、ステータスが「新規」に戻ります。
* **拒否されたリクエストの推奨ステータス：** 前のステータス（「新規」）に戻すのではなく、「解決されません」などの別のステータスを選択して、混乱を避けることをお勧めします。
* **カスタムステータスオプション：** デフォルトでは「却下」ステータスは提供されていませんが、承認プロセスをより明確にするために必要に応じて、システム管理者が作成できます。


## このトピックに関する推奨チュートリアル

* [タスク、イシュー、承認を委任する](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)
* [グループ特有の承認プロセスについて](/help/administration-and-setup/approval-processes-and-milestone-paths/group-specific-approval-processes.md)
* [リクエストフローの作成](/help/manage-work/request-queues/create-a-request-flow.md)
* [ グローバルおよび単一使用の承認プロセスの作成 ](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)
