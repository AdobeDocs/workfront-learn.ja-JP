---
title: 配達確認に関するレポート
description: レポート機能を使用して配達確認の進行状況を管理する方法を説明します。
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: report-on-proofs.png
kt: 10233
exl-id: 9a1a9e16-61cc-4f95-977a-8870b7fd0dda
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# 配達確認に関するレポート

[!DNL Workfront]のデジタル校正機能を使用すると、プロジェクトと関連するレビューワークフローを 1 か所で管理できます。 [!DNL Workfront]. レビューおよび承認情報を表示するレポートの種類、フィールドソース、フィールド名を使用して行われる校正作業に関する有益な情報を得ます。

を [!DNL Workfront] コンサルタントに問い合わせて、組織の要件を満たすレポートを作成してもらいます。 一部のレポートでは、 [!DNL Workfront]のテキストモードレポート。

これらの基本的な標準レポートを使用して、チームが [!DNL Workfront].

## [!UICONTROL プルーフの承認]

このレポートタイプを使用すると、未処理の配達確認の承認を追跡して、期限を満たしていることを確認できます。

![選択 [!UICONTROL 配達確認の承認] から [!UICONTROL 新しいレポート] ドロップダウンメニュー](assets/proof-system-setups-proof-approval-report.png)

表示およびフィルターのオプションは次のとおりです [!UICONTROL 決定日], [!UICONTROL 配達確認の承認], [!UICONTROL 承認段階], [!UICONTROL ワークフローテンプレート]、および [!UICONTROL 請求者情報]. テキストモードのレポートを使用すると、ドキュメント名でリストを整理するグループ化を作成できます。

配達確認の承認レポートを作成する場合は、配達確認の最新バージョンに関する情報を取得していることを確認してください。 [!DNL Workfront] では、このフィールドのソースとフィールド名をフィルターに含めることをお勧めします。

**[!UICONTROL 配達確認の承認]>>[!UICONTROL 現在のドキュメントのバージョン]**

![Report Builder の「フィルター」タブ](assets/proof-system-setups-proof-approval-report-is-current-version.png)

これは、複数のバージョンを持つ配達確認のレポートで、承認が必要な各配達確認の現在のバージョンのみがレポートに表示されるようにする場合に役立ちます。 これにより、作業する必要がなくなった以前のバージョンが除外されます。

## [!UICONTROL ドキュメント バージョン]

このレポートタイプでは、 [!DNL Workfront].

![選択 [!UICONTROL ドキュメントのバージョン] から [!UICONTROL 新しいレポート] ドロップダウンメニュー](assets/proof-system-setups-document-version-report.png)

表示オプションには、 [!UICONTROL ドキュメントバージョン], [!UICONTROL 文書], [!UICONTROL 入力者], [!UICONTROL 配達確認の承認ステータス], [!UICONTROL 配達確認作成者]、および [!UICONTROL ドキュメントプロバイダー].

グループ化は、次の方法で実行できます [!UICONTROL ドキュメントバージョン], [!UICONTROL 入力者], [!UICONTROL 配達確認の承認ステータス]、または配達確認の所有者情報。

次を含むフィルター [!UICONTROL ドキュメントバージョン], [!UICONTROL アクセスレベル], [!UICONTROL 文書], [!UICONTROL 入力者], [!UICONTROL 配達確認の承認ステータス], [!UICONTROL 配達確認作成者]、およびドキュメントプロバイダーの情報。

レポートの各文書に対して現在アクティブな校正ステージの名前を、この列でビューに表示できます。

**[!UICONTROL ドキュメントのバージョン] >> [!UICONTROL アクティブな配達確認ステージ]**

![Report Builder の「フィルター」タブ](assets/proof-system-setups-active-proof-stages.png)

現在アクティブなステージがない場合、列は空白になります。

このフィールドソース/> フィールド名は、レポートのフィルターとしても使用できます。

以下を使用： [!UICONTROL 配達確認の作成者] フィールドのソース：配達確認を作成したユーザーに関する情報をレポートします。 を選択します。 [!UICONTROL 名前] ビューに配達確認の作成者の名前を表示するフィールドソース。

**[!UICONTROL 配達確認の作成者] >> [!UICONTROL 名前]**

このフィールドソース/> フィールド名のコンボは、フィルターとしても使用できます。

![Report Builder の「フィルター」タブ](assets/proof-system-setups-proof-creator-name.png)

<!--
Learn More Icon
Learn how to create reports in [!DNL Workfront] with the Report Creation class.
Access to proofing functionality
-->
