---
title: パフォーマンス指標について
description: '[!UICONTROL パフォーマンスインデックスメソッド]（[!UICONTROL PIM]）と[!UICONTROL 完了時の見積もり]（[!UICONTROL EAC]）のパフォーマンス指標の使用方法について説明します。'
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-performance-metrics.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10065
exl-id: 190c66f5-b412-48bd-8695-3bd7da088ccb
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 100%

---

# パフォーマンス指標について

プロジェクト管理者が使用する 2 つのパフォーマンス指標には、[!UICONTROL パフォーマンスインデックスメソッド]（[!UICONTROL PIM]）と[!UICONTROL 完了時の見積もり]（[!UICONTROL EAC]）があります。システム全体のデフォルトは [!DNL Workfront] で設定でき、新しく作成したプロジェクトに適用します。その後、個々のプロジェクトで [!UICONTROL PIM] を変更できます。

**[!UICONTROL PIM]**

[!UICONTROL PIM] の設定は、[!DNL Workfront] で[!UICONTROL コストパフォーマンスインデックス]（[!UICONTROL CPI]）、[!UICONTROL コストスケジュールパフォーマンスインデックス]（[!UICONTROL CSI]）、[!UICONTROL スケジュールパフォーマンスインデックス]（[!UICONTROL SPI]）、[!UICONTROL 完了時の見積もり]（[!UICONTROL EAC]）などの他のプロジェクトパフォーマンス指標を計算する方法をコントロールします。

[!UICONTROL PIM] のオプションは、時間ベースとコストベースです。

* **時間ベース** - Workfront では、プロジェクトの CPI と EAC を計算する際に予定時間数を使用します。プロジェクトの EAC は、時間単位の数値として表示されます。
* **コストベース** - Workfront では、プロジェクトの CPI と EAC の計算に予定労力コストを使用します。EAC は、通貨値として表示されます。このオプションを使用する場合は、タスクの担当者（ユーザーや担当業務）がコスト率に関連付けられていることを確認します。

**[!UICONTROL 完成時総コスト見積り (EAC)]**

[!UICONTROL EAC] は、タスクまたはプロジェクトが完了すると見込まれる合計コストを表します。オプションは、プロジェクトレベルで計算され、タスク／サブタスクからロールアップされます。

* **プロジェクトレベルでの計算** - 親タスクとプロジェクトの [!UICONTROL EAC] は、[!UICONTROL EAC] 式の実際の時間数／実際の労力コストを使用して決定されます。計算には、親タスクまたはプロジェクトに直接追加された実際の時間数／コストと費用が含まれます。
* **タスク／サブタスクからのロールアップ** - 親タスクとプロジェクトの [!UICONTROL EAC] は、各子タスクの [!UICONTROL EAC] を合計することによって決定されます。この計算では、親タスクまたはプロジェクトに直接追加された実際の時間数／コストは除外されます。

[!UICONTROL EAC] の計算は、[完成時総コスト見積もり（EAC）の計算](https://experienceleague.adobe.com/docs/workfront/using/manage-work/projects/project-finances/calculate-eac.html?lang=ja)に記載されています。

**パフォーマンス指標：設定**

[!UICONTROL PIM] および [!UICONTROL EAC] システムのデフォルトを設定するには：

1. メインメニューから「**[!UICONTROL 設定]**」を選択します。
1. 左側のパネルメニューで「**[!UICONTROL プロジェクト環境設定]**」をクリックし、「**[!UICONTROL プロジェクト]**」をクリックします
1. 「[!UICONTROL プロジェクトステータス]」セクションで、[!UICONTROL パフォーマンスインデックスメソッド]を検索します。「時間ベース」または「コストベース」を選択します。
1. [!UICONTROL 完了時の見積もり]については、プロジェクトレベルでの「計算」またはタスク／サブタスクからの「ロールアップ」を選択します。
1. ウィンドウの下部にある「**[!UICONTROL 保存]**」をクリックします。

![[!UICONTROL プロジェクト環境設定]画面の画像](assets/setting-up-finances-1.png)

**個々のプロジェクトでの [!UICONTROL PIM] の設定**

1. プロジェクトのランディングページに移動します。
1. 左側のパネルから「**[!UICONTROL プロジェクト詳細]**」をクリックします。
1. 「**[!UICONTROL 財務]**」セクションを開きます。
1. **[!UICONTROL パフォーマンスインデックスメソッド]**&#x200B;の下にあるテキストをダブルクリックして編集します。
1. 「時間ベース」または「コストベース」を選択します。
1. 「**[!UICONTROL 変更を保存]**」をクリックして終了します。

![[!UICONTROL プロジェクト詳細]画面の画像](assets/setting-up-finances-2.png)

[!UICONTROL PIM] は、プロジェクトテンプレートのテンプレート詳細の「[!UICONTROL 財務]」セクションで設定できます。
