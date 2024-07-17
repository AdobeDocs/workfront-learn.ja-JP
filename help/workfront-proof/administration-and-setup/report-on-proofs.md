---
title: プルーフに関するレポート
description: レポーティングを使用してプルーフの進捗状況を管理する方法について説明します。
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: report-on-proofs.png
jira: KT-10233
exl-id: 9a1a9e16-61cc-4f95-977a-8870b7fd0dda
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 100%

---

# プルーフに関するレポート

[!DNL Workfront] のデジタルプルーフ機能を使用すると、プロジェクトと関連するレビューワークフローを [!DNL Workfront] で一元管理できます。レビューおよび承認情報を表示するレポートタイプ、フィールドソース、フィールド名を使用して行なわれるプルーフ作業に関する有益な情報を得ます。

[!DNL Workfront] コンサルタントと協力して、組織の要件を満たすレポートを作成することをお勧めします。一部のレポートでは、[!DNL Workfront] のテキストモードレポーティングに関する十分な知識が必要です。

これらの基本的で標準的なレポートから始めて、チームが [!DNL Workfront] のレビューと承認プロセスを経たプルーフを管理できるようにします。

## [!UICONTROL プルーフの承認]

このレポートタイプを使用すると、未処理のプルーフの承認を追跡して、期限を満たしていることを確認できます。

![[!UICONTROL 新しいレポート]ドロップダウンメニューから「[!UICONTROL プルーフの承認]」を選択する](assets/proof-system-setups-proof-approval-report.png)

表示およびフィルターのオプションには、[!UICONTROL 決定日]、[!UICONTROL プルーフの承認]、[!UICONTROL 承認者ステージ]、[!UICONTROL ワークフローテンプレート]、[!UICONTROL 依頼者情報]が含まれます。テキストモードのレポートを使用すると、ドキュメント名でリストを整理するグループ化を作成できます。[グループ化の基本的なテキストモードについて](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/basic-text-mode-for-groupings.html?lang=ja)を参照してください。

プルーフの承認レポートを作成する際は、プルーフの現在のバージョンに関する情報を取得していることを確認してください。[!DNL Workfront] では、このフィールドのソースとフィールド名をフィルターに含めることをお勧めします。

**[!UICONTROL プルーフの承認]／[!UICONTROL 現在のドキュメントのバージョン]**

![Report Builder の「フィルター」タブ](assets/proof-system-setups-proof-approval-report-is-current-version.png)

承認が必要な各プルーフの最新バージョンのみがレポートにリストされるため、複数のバージョンがあるプルーフのレポートに便利です。これにより、作業する必要がなくなった以前のバージョンが除外されます。

## [!UICONTROL ドキュメント バージョン]

このレポートタイプを使用すると、[!DNL Workfront] でバージョンを管理および追跡することができます。

![[!UICONTROL 新しいレポート]ドロップダウンメニューから「[!UICONTROL ドキュメントバージョン]」を選択する](assets/proof-system-setups-document-version-report.png)

表示オプションには、[!UICONTROL ドキュメントバージョン]、[!UICONTROL ドキュメント]、[!UICONTROL 入力者]、[!UICONTROL プルーフ承認ステータス]、 [!UICONTROL プルーフ作成者]、[!UICONTROL ドキュメント提供者]の情報が含まれます。

グループ化は、[!UICONTROL ドキュメントバージョン]、[!UICONTROL 入力者]、[!UICONTROL プルーフ承認ステータス]、プルーフ所有者情報によって行うことができます。

フィルターには、[!UICONTROL ドキュメントバージョン]、[!UICONTROL アクセスレベル]、[!UICONTROL ドキュメント]、[!UICONTROL 入力者]、[!UICONTROL プルーフ承認ステータス]、[!UICONTROL プルーフ作成者]、ドキュメント提供者の情報が含まれます。

ビューのこの列を使用して、レポートの各ドキュメントで現在アクティブなプルーフステージの名前を表示できます。

**[!UICONTROL ドキュメントのバージョン]／[!UICONTROL アクティブなプルーフステージ]**

![Report Builder の「フィルター」タブ](assets/proof-system-setups-active-proof-stages.png)

現在アクティブなステージがない場合、列は空白になります。

このフィールドソース >>フィールド名は、レポートのフィルターとしても使用できます。

「[!UICONTROL プルーフ作成者]」フィールドソースを使用して、プルーフを作成したユーザーに関する情報をレポートします。ビューにプルーフ作成者の名前を表示するには、[!UICONTROL 名前]フィールドソースを選択します。

**[!UICONTROL プルーフの作成者]／[!UICONTROL 名前]**

このフィールドソース／フィールド名の組み合わせは、フィルターとしても使用できます。

![Report Builder の「フィルター」タブ](assets/proof-system-setups-proof-creator-name.png)

<!--
Learn More Icon
Learn how to create reports in [!DNL Workfront] with the Report Creation class.
Access to proofing functionality
-->
