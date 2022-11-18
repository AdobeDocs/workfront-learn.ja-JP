---
title: パフォーマンス指標について
description: パフォーマンス指標の使用方法を説明します。 [!UICONTROL パフォーマンスインデックスメソッド] ([!UICONTROL PIM]) および [!UICONTROL 完了時の推定] ([!UICONTROL EAC]) をクリックします。
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-performance-metrics.png
type: Tutorial
role: User
level: Intermediate
kt: 10065
exl-id: 190c66f5-b412-48bd-8695-3bd7da088ccb
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# パフォーマンス指標について

プロジェクトマネージャーが使用する 2 つのパフォーマンス指標には、 [!UICONTROL パフォーマンスインデックスメソッド] ([!UICONTROL PIM]) および [!UICONTROL 完了時の推定] ([!UICONTROL EAC]) をクリックします。 システム全体のデフォルト値は、 [!DNL Workfront] 新しく作成されたプロジェクトに適用します。 [!UICONTROL PIM] その後、個々のプロジェクトで変更できます。

**[!UICONTROL パ イ メ]**

の設定 [!UICONTROL PIM] ～を制御する [!DNL Workfront] 次のような他のプロジェクト効果指標を計算します。 [!UICONTROL コスト効果指数] ([!UICONTROL CPI]), [!UICONTROL 原価計画実績インデックス] ([!UICONTROL CSI]), [!UICONTROL スケジュール効果インデックス] ([!UICONTROL SPI]) および [!UICONTROL 完了時の推定] ([!UICONTROL EAC]) をクリックします。

のオプション [!UICONTROL PIM] は時間ベースとコストベースです。

* **時間ベース** Workfrontは、計画時間を使用して、CPI と EAC を算出している。 プロジェクトの EAC は、数値（時間単位）で表示されます。
* **コストベース** Workfront氏は、CPI と EAC の算出に、計画された人件費を使用している。 EAC は通貨値として表示されます。 このオプションを使用する場合は、タスクの担当者（ユーザーやジョブの役割）がコスト率に関連付けられていることを確認します。

**[!UICONTROL 完成時総コスト見積り (EAC)]**

[!UICONTROL EAC] タスクまたはプロジェクトの完了時の推定総コストを表します。 オプションは、プロジェクトレベルで計算され、タスク/サブタスクからロールアップされます。

* **プロジェクトレベルで計算** — [!UICONTROL EAC] 親タスクとプロジェクトの場合、実際の時間/実際の人件費を使用して、 [!UICONTROL EAC] 式。 計算には、実際の時間/コストと費用が、親タスクまたはプロジェクトに直接追加されます。
* R **タスク/サブタスクからのロールアップ** — [!UICONTROL EAC] 親タスクとプロジェクトの場合、 [!UICONTROL EAC] 各子タスク この計算では、親タスクまたはプロジェクトに直接追加された実際の時間/コストは除外されます。

この [!UICONTROL EAC] 計算は、「完了時の見積もりの計算 (EAC)」にリストされます。 <!-- link to article -->記事 [!UICONTROL [!DNL Workfront] 1].

**パフォーマンス指標：設定**

設定するには [!UICONTROL PIM] および [!UICONTROL EAC] システムのデフォルト：

1. 選択 **[!UICONTROL 設定]** を選択します。
1. クリック **[!UICONTROL プロジェクト環境設定]** 左側のパネルメニューで、 **[!UICONTROL プロジェクト]**
1. 内 [!UICONTROL プロジェクトステータス] セクション、検索 [!UICONTROL パフォーマンスインデックスメソッド]. 「時間ベース」または「コストベース」を選択します。
1. の場合 [!UICONTROL 完了時の推定]、「プロジェクトレベルで計算」または「タスク/サブタスクからロールアップ」を選択します。
1. クリック **[!UICONTROL 保存]** 窓の下に

![画像 [!UICONTROL プロジェクト環境設定] screen](assets/setting-up-finances-1.png)

**設定 [!UICONTROL PIM] 個々のプロジェクトで**

1. プロジェクトのランディングページに移動します。
1. クリック **[!UICONTROL プロジェクトの詳細]** を左側のパネルからクリックします。
1. を開きます。 **[!UICONTROL 金融]** 」セクションに入力します。
1. 下のテキストをダブルクリックします。 **[!UICONTROL パフォーマンスインデックスメソッド]** をクリックして編集します。
1. 「時間ベース」または「コストベース」を選択します。
1. クリック **[!UICONTROL 保存]** 変更が完了しました。

![画像 [!UICONTROL プロジェクトの詳細] screen](assets/setting-up-finances-2.png)

[!UICONTROL PIM] は、プロジェクトテンプレートの [!UICONTROL 金融] 」セクションに表示されます。
