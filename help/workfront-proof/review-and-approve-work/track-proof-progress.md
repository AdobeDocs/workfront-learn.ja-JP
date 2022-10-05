---
title: 配達確認の進行状況の追跡方法
description: 使用方法を学ぶ [!UICONTROL SOCD] 配達確認の進行状況をトラッキングする指標、配達確認の進行状況およびレポート ( [!DNL  Workfront].
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: track-proof-progress.png
kt: 10111
exl-id: 343483fe-487a-4a23-914d-2807a00630f9
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 1%

---

# 配達確認の進行状況を追跡

プロジェクトマネージャー、配達確認マネージャーまたはレビューおよび承認プロセスのその他の関係者として、配達確認の進行状況をトラッキングする必要があります。 これをおこなうには、 [!DNL Workfront’s] 組み込み **配達確認の進行状況インジケーター** の [!UICONTROL ドキュメント] ページ内で、またはカスタムレポートを作成することで、個別のレポートを作成できます。

配達確認の進行状況を表示するには [!DNL Workfront]、プラン、作業、レビューのライセンスを持ち、校正ユーザーである必要があります。 もし、 [!DNL Workfront] プロファイルがこれらの要件を満たしている場合は、組織の校正システム管理者に問い合わせてください。

## 次を使用して配達確認の進行状況を追跡 [!UICONTROL SOCD] 指標と配達確認のステータス

レビューおよび承認プロセスの進行状況を、 [!UICONTROL SOCD] アイコン [!UICONTROL ドキュメント] リスト。 これらのアイコンは、配達確認に対して実行された特定のアクションを示します。

![画像 [!UICONTROL ドキュメント] リスト [!DNL  Workfront] プロジェクトを [!UICONTROL SOCD] 強調表示されたアイコン。](assets/manage-proofs-socd.png)

アイコンは、配達確認を受信者に送信した時点から配達確認を決定した時点までの配達確認に対する作業を示します。

* **S —** 配達確認が受信者に送信されました。
* **O —** 配達確認が開かれました。
* **C —** 配達確認に対するコメントが行われました。
* **D —** 配達確認に関する決定がおこなわれました（承認、却下など）。

色は、アクションが完了したかどうかを示します。

* **白 —** まだステップが発生していません。
* **緑 —** 手順が完了しました。
* **オレンジ —** 配達確認の期限は 24 時間以内で、手順は実行されません。
* **赤 —** 配達確認の期限が過ぎ、ステップは実行されません。

この [!UICONTROL SOCD] の [!UICONTROL ドキュメント] リスト、概要パネル、または [!UICONTROL ドキュメントの詳細]は、配達確認の進行状況の概要です。 [!DNL Workfront] は、校正プロセスで「最も遅れている」受信者に基づいてこれを設定します。

例えば、3 人のレビュー担当者/承認者がいて、そのうち 2 人だけが配達確認を閲覧してコメントを行った場合、 [!UICONTROL SOCD] アイコンは、配達確認が送信されたことを示します ([!UICONTROL S]) および開かれた ([!UICONTROL O]) が作成されたが、コメントは作成されていない ([!UICONTROL C]) をクリックします。

個々の配達確認の受信者の行動を把握するには、校正ワークフローを開きます。 配達確認の全体的な進行状況は、ウィンドウの上部に表示されます。 各ステージには、灰色のバーに独自の進行状況インジケーターが表示されます。  各ユーザーの横には、その個人の進歩が表示されます。

![画像 [!UICONTROL 校正ワークフロー] セクションに含める必要があります。](assets/manage-proofs-socd-in-proofing-workflow-window.png)

## 配達確認のステータス

配達確認のステータスは、ステージの配達確認受信者のステータスに基づきます。 配達確認の全体的なステータスは、 [!UICONTROL ドキュメント] ページの右側にある [!UICONTROL SOCD] 指標を使用することで、配達確認に関する決定があるかどうかを簡単に判断できます。

![画像 [!UICONTROL ドキュメント] リスト [!DNL  Workfront] プロジェクトの全体的な配達確認ステータスがハイライト表示されます。](assets/manage-proofs-overall-status.png)

この配達確認のステータスは、配達確認の全体的なステータスを示します。 例えば、2 人の受信者が配達確認を承認した場合、個々のステータスが表示されます [!UICONTROL 承認済み]. ただし、3 人目の受信者はまだ決定していないので、ステータスは「 [!UICONTROL 保留中]. したがって、全体のステータスは次のように表示されます。 [!UICONTROL 保留中].

組織に対してカスタムステータスが設定されている場合は、それらのステータスが使用されます。 それ以外の場合は、次の標準ステータスオプションが表示されます。

* [!UICONTROL 保留中]
* [!UICONTROL 承認済み]
* [!UICONTROL 変更も承認済み]
* [!UICONTROL 変更が必要です]
* [!UICONTROL 無関係]

校正ワークフローウィンドウを開き、 [!UICONTROL レビュー担当者と承認者] または [!UICONTROL 承認者 ]配達確認の役割。

## のレポート [!DNL Workfront]

また、 [!DNL Workfront’s] レビューおよび承認プロセスを進行するたびに配達確認を追跡するレポート機能

配達確認の承認レポートを使用すると、未処理の承認を追跡して、期限を満たしていることを確認できます。

![の配達確認承認レポートの画像 [!DNL  Workfront].](assets/proof-approval-report.png)

ドキュメントのバージョンレポートでは、配達確認のバージョンを管理および追跡できます。

![のドキュメントバージョンレポートの画像 [!DNL  Workfront].](assets/document-version-report.png)

を [!DNL Workfront] コンサルタントに問い合わせて、組織の要件を満たすレポートを作成してもらいます。 一部のレポートでは、 [!DNL Workfront’s] テキストモードのレポート。

## あなたのターン

配達確認ワークフローをスムーズに実行するためにWorkfrontで使用するレポートの種類については、チームまたは校正システム管理者にお問い合わせください。

<!--
### Learn more
* Learn to create reports in [!DNL Workfront] with the Basic Report Creation course.
* View progress and status of a proof
* View activity on a proof within [!DNL Workfront]
-->
