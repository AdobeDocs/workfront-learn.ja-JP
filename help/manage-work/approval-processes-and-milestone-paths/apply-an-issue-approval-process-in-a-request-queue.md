---
title: リクエストキューへのイシュー承認プロセスの適用
description: デフォルトの承認プロセスを実装して、リクエストのワークフローを効率化します。これにより、承認済みリクエストのステータスが適切に「新規」に変更されます。 「解決されない」に対するステータスの変更を選択して、却下されたリクエストの混乱に対処します。
activity: use
feature: Approvals
thumbnail: 335225.jpeg
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-17578
last-substantial-update: '2025-03-26T00:00:00.000Z'
recommendations: noDisplay,catalog
doc-type: video
exl-id: 9200eeb4-db5d-45c1-9b17-28c6ca04de2d
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: c10f2e93-7a58-4212-aa24-684c265ebe76
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-06T15:58:59.618Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 426
ht-degree: 65%

---

# リクエストキューへのイシュー承認プロセスの適用

>[!PREREQUISITES]
>
>* [リクエストフローの作成](https://experienceleague.adobe.com/ja/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/create-a-request-flow)
>* [グローバルおよび単一使用承認プロセスの作成](https://experienceleague.adobe.com/ja/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)


このビデオでは、リクエストキューを作成する際にデフォルトの承認プロセスを適用するプロセスについて説明します。 &#x200B; リクエストが作成されると、ステータス「新規 – 承認保留中」で開始され、承認通知が指定された承認者に送信されます。 &#x200B;承認されると、ステータスは「新規」に変わり、割り当てられた個人が作業を開始できるようになります。 &#x200B;却下された場合、承認プロセスの設定でよくある間違いにより、ステータスが「新規」に誤って戻る可能性があります。 &#x200B;
このビデオでは、ステータスが「新規」に設定されている場合に承認プロセスがトリガーされることを強調しています。これは、新規リクエストのデフォルトです。 &#x200B;拒否された場合、システムはデフォルトでステータスを前のステータスに戻します。これは新しいリクエストには適していません。 代わ&#x200B;、「解決しない」などの別のステータスを選択する必要があります。 &#x200B;このビデオでは、デフォルトで「却下」ステータスが提供されていないことにも注意していますが、必要に応じてシステム管理者がステータスを作成できます。 &#x200B;

>[!VIDEO](https://video.tv.adobe.com/v/3455013/?quality=12&learn=on&enablevpops=1)

## 重要な留意点

* **デフォルトの承認プロセス：**&#x200B;リクエストキューの作成時に、各リクエストに承認ワークフローを自動的に割り当てるデフォルトの承認プロセスを適用できます。
* **承認時のステータス変更：**&#x200B;承認済みリクエストのステータスは「新規 - 承認を保留中」から「新規」に変更され、割り当てられた個人が作業を開始できます。
* **却下処理での一般的な間違い：**&#x200B;リクエストが却下された場合、承認プロセスのデフォルトのシステム設定により、ステータスは「新規」に戻ります。
* **却下するリクエストの推奨ステータス：**&#x200B;混乱を回避するために、以前のステータス（「新規」）に戻すのではなく、「解決されない」などの別のステータスを選択することをお勧めします。
* **カスタムステータスオプション：**&#x200B;デフォルトで「却下」ステータスは提供していませんが、承認プロセスをより明確にするために、必要に応じてシステム管理者がステータスを作成できます。


## このトピックに関する推奨チュートリアル

* [タスク、イシュー、承認の委任](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)
* [グループ特有の承認プロセスについて](/help/administration-and-setup/approval-processes-and-milestone-paths/group-specific-approval-processes.md)
* [リクエストフローの作成](/help/manage-work/request-queues/create-a-request-flow.md)
* [グローバルおよび単一使用承認プロセスの作成](https://experienceleague.adobe.com/ja/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)
