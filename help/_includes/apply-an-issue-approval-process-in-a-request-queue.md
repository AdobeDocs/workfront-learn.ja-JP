---
source-git-commit: b150105844a42e06f5e96f787ad62a1b62185f91
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 51%

---
# リクエストキューでのイシュー承認プロセスの適用 – 共有

>[!PREREQUISITES]
>
>* [Workfrontでリクエストフローを作成](https://experienceleague.adobe.com/ja/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/create-a-request-flow)
>* [承認プロセスの作成と管理](https://experienceleague.adobe.com/ja/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)


このビデオでは、リクエストキューを作成する際にデフォルトの承認プロセスを適用するプロセスについて説明します。 &#x200B; リクエストが作成されると、ステータス「新規 – 承認保留中」で開始され、承認通知が指定された承認者に送信されます。 &#x200B;承認されると、ステータスは「新規」に変わり、割り当てられた個人が作業を開始できるようになります。 &#x200B;却下された場合、承認プロセスの設定でよくある間違いにより、ステータスが「新規」に誤って戻る可能性があります。 &#x200B;
このビデオでは、ステータスが「新規」に設定されている場合に承認プロセスがトリガーされることを強調しています。これは、新規リクエストのデフォルトです。 &#x200B;拒否された場合、システムはデフォルトでステータスを前のステータスに戻します。これは新しいリクエストには適していません。 代わ&#x200B;、「解決しない」などの別のステータスを選択する必要があります。 &#x200B;このビデオでは、デフォルトで「却下」ステータスが提供されていないことにも注意していますが、必要に応じてシステム管理者がステータスを作成できます。 &#x200B;

>[!VIDEO](https://video.tv.adobe.com/v/3455025/?captions=jpn&quality=12&learn=on&enablevpops=1)

## 重要な留意点

* **デフォルトの承認プロセス：**&#x200B;リクエストキューの作成時に、各リクエストに承認ワークフローを自動的に割り当てるデフォルトの承認プロセスを適用できます。
* **承認時のステータス変更：**&#x200B;承認済みリクエストのステータスは「新規 - 承認を保留中」から「新規」に変更され、割り当てられた個人が作業を開始できます。
* **却下処理での一般的な間違い：**&#x200B;リクエストが却下された場合、承認プロセスのデフォルトのシステム設定により、ステータスは「新規」に戻ります。
* **却下するリクエストの推奨ステータス：**&#x200B;混乱を回避するために、以前のステータス（「新規」）に戻すのではなく、「解決されない」などの別のステータスを選択することをお勧めします。
* **カスタムステータスオプション：**&#x200B;デフォルトで「却下」ステータスは提供していませんが、承認プロセスをより明確にするために、必要に応じてシステム管理者がステータスを作成できます。


## このトピックに関する推奨チュートリアル

* [タスク、イシュー、承認の効果的な委任](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)
* [グループ固有の承認プロセスについて](/help/administration-and-setup/approval-processes-and-milestone-paths/group-specific-approval-processes.md)
* [Workfrontでのリクエストフローの作成](/help/manage-work/request-queues/create-a-request-flow.md)
* [承認プロセスの作成と管理](https://experienceleague.adobe.com/ja/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)

