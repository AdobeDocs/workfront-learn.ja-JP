---
title: プルーフの進捗状態を追跡する
description: '[!UICONTROL SOCD] インジケーター、プルーフの進捗状況、レポートを使用して、 [!DNL  Workfront] でプルーフの進捗状況を追跡する方法を学びます。'
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: track-proof-progress.png
jira: KT-10111
exl-id: 343483fe-487a-4a23-914d-2807a00630f9
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '675'
ht-degree: 100%

---

# プルーフの進捗状態を追跡する

プロジェクトマネージャー、プルーフマネージャー、レビューおよび承認プロセスでのその他の関係者は、プルーフの進捗状況を追跡する必要があります。 これを行うには、[!UICONTROL ドキュメント]ページの[!DNL Workfront’s]ビルトイン&#x200B;**プルーフ進捗状態インジケーター**&#x200B;を使用するか、カスタムレポートを作成します。

[!DNL Workfront] でプルーフの進捗状況を表示するには、プラン、ワーク、またはレビューのライセンスを保有し、かつプルーフユーザーである必要があります。 [!DNL Workfront] プロファイルがこれらの要件を満たしているかどうかが不明な場合は、組織のプルーフシステム管理者にお問い合わせください。

## [!UICONTROL SOCD] インジケーターとプルーフステータスでプルーフの進捗状況を追跡する

[!UICONTROL ドキュメント]リストの [!UICONTROL SOCD] アイコンを使用して、プルーフがレビューと承認プロセスでどのように進行しているかの概要を表示します。これらのアイコンは、プルーフに対して実行された特定のアクションを示します。

![[!UICONTROL SOCD] アイコンが強調表示された、[!DNL  Workfront]プロジェクトの[!UICONTROL ドキュメント]リストの画像](assets/manage-proofs-socd.png)

アイコンは、プルーフを受信者に送信してから受信者がプルーフで決定を下すまでに、プルーフで行われた作業を示します。

* **S**：プルーフが受信者に送信されました。
* **O**：プルーフが開かれました。
* **C**：プルーフにコメントが付けられました。
* **D**：プルーフに関する決定が下されました（承認、却下など）。

色は、アクションが完了したかどうかを示します。

* **白**： まだステップが発生していません。
* **緑**：ステップが完了しました。
* **橙**：プルーフの期限は 24 時間以内ですが、ステップが実行されていません。
* **赤**：プルーフの期限が過ぎましたが、ステップが実行されていません。

[!UICONTROL ドキュメント]リスト、概要パネル、[!UICONTROL ドキュメントの詳細]にある [!UICONTROL SOCD] は、 プルーフの進捗状態です。[!DNL Workfront] では、プルーフプロセスで「最も遅れている」受信者に基づいてこれを設定します。

例えば、3 人のレビュアー／承認者がいて、そのうち 2 人だけがプルーフを閲覧してコメントを付けた場合、[!UICONTROL SOCD] アイコンは、プルーフが送信され（[!UICONTROL S]）て開かれた（[!UICONTROL O]）ことを示しますが、コメントが作成された（[!UICONTROL C]）ことは示しません。

個々のプルーフ受信者の行動を把握するには、プルーフワークフローを開きます。 プルーフの全体的な進捗状況は、ウィンドウの上部に表示されます。 各ステージには、灰色のバーに独自の進捗状況インジケーターが表示されます。  各ユーザーの横には、その個人の進捗が表示されます。

![ドキュメントの[!UICONTROL プルーフワークフロー]セクションの画像。](assets/manage-proofs-socd-in-proofing-workflow-window.png)

## プルーフのステータス

プルーフのステータスは、ステージのプルーフ受信者のステータスに基づきます。 [!UICONTROL SOCD] インジケーターの右側にある[!UICONTROL ドキュメント]ページに全体的なプルーフステータスが表示されるため、プルーフに関する決定があるかどうかを簡単に確認できます。

![全体的なプルーフステータスが強調表示されている、[!DNL  Workfront]プロジェクトの[!UICONTROL ドキュメント]リストの画像](assets/manage-proofs-overall-status.png)

このプルーフのステータスは、プルーフの全体的なステータスを示します。 例えば、2 人の受信者がプルーフを承認した場合、個々のステータスが[!UICONTROL 承認済み]として示されます。ただし、3 人目の受信者はまだ決定していないので、そのユーザーのステータスは[!UICONTROL 保留中]になります。したがって、全体のステータスは[!UICONTROL 保留中]になります。

組織に対してカスタムステータスが設定されている場合は、それらのステータスが使用されます。 それ以外の場合は、次の標準ステータスオプションが表示されます。

* [!UICONTROL 保留中]
* [!UICONTROL 承認済み]
* [!UICONTROL 変更も承認済み]
* [!UICONTROL 変更が必要です]
* [!UICONTROL 無関係]

プルーフワークフローウィンドウを開いて、プルーフの[!UICONTROL レビュアーおよび承認者]または[!UICONTROL 承認者]の役割が割り当てられた受信者のプルーフステータスを確認します。

## [!DNL Workfront] のレポート

また、[!DNL Workfront’s] レポート機能を活用して、レビューと承認のプロセスを経てプルーフを追跡することもできます。

プルーフ承認レポートを使用すると、未処理の承認を追跡して、期限に間に合わせることができます。

![[!DNL  Workfront] のプルーフ承認レポートの画像](assets/proof-approval-report.png)

ドキュメントのバージョンレポートでは、プルーフのバージョンを管理および追跡できます。

![[!DNL  Workfront] のドキュメントのバージョンレポートの画像 ](assets/document-version-report.png)

[!DNL Workfront] コンサルタントと協力して、組織の要件を満たすレポートを作成することをお勧めします。一部のレポートでは、[!DNL Workfront’s] テキストモードレポートの知識が必要です。

## やってみよう

チームまたプルーフシステム管理者と相談して、プルーフワークフローをスムーズに実行するために Workfront で使用するレポートの種類を確認してください。

<!--
### Learn more
* Learn to create reports in [!DNL Workfront] with the Basic Report Creation course.
* View progress and status of a proof
* View activity on a proof within [!DNL Workfront]
-->
