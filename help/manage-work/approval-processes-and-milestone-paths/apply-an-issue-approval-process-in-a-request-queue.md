---
title: リクエストキューへのイシュー承認プロセスの適用
description: デフォルトの承認プロセスを実装して、リクエストのワークフローを効率化します。これにより、承認済みリクエストのステータスが適切に「新規」に変更されます。「解決されない」に対するステータスの変更を選択して、却下されたリクエストの混乱に対処します。
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
exl-id: 9200eeb4-db5d-45c1-9b17-28c6ca04de2d
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 100%

---

# リクエストキューへのイシュー承認プロセスの適用

>[!PREREQUISITES]
>
>* [リクエストフローの作成](https://experienceleague.adobe.com/ja/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/create-a-request-flow)
>* [グローバルおよび単一使用承認プロセスの作成](https://experienceleague.adobe.com/ja/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)


ビデオでは、リクエストキューの作成時にデフォルトの承認プロセスを適用するプロセスについて説明します。リクエストを作成すると、ステータスは「新規 - 承認を保留中」から開始され、指定した承認者に承認通知が送信されます。承認された場合、ステータスが「新規」に変更され、割り当てられた個人が作業を開始できます。却下された場合、承認プロセスの設定での一般的な間違いにより、ステータスが誤って「新規」に戻る場合があります。
ビデオでは、ステータスが「新規」に設定されると承認プロセスがトリガーされることをハイライト表示しています。これは、新しいリクエストのデフォルトです。却下された場合、デフォルトでステータスが以前の状態に戻されますが、これは新しいリクエストには適していません。代わりに、「解決されない」などの別のステータスを選択する必要があります。また、ビデオでは、デフォルトで「却下」ステータスを提供していませんが、必要に応じてシステム管理者がステータスを作成できることも説明しています。

>[!VIDEO](https://video.tv.adobe.com/v/3455013/?quality=12&learn=on&enablevpops=1)

## 主な要点

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
