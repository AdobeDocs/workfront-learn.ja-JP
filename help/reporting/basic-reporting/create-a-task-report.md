---
title: タスクレポートの作成
description: 複雑なフィルターを使用してタスクレポートを作成し、Workfront で作成したレポートを見つける方法について説明します。アクティビティ - プロンプト付きのメモレポートを作成します。
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335154.png
jira: KT-8859
exl-id: 90bad2e8-9cd2-4ae7-973b-eeab9d615bef
doc-type: video
source-git-commit: 2134c921e39a549808bb11235b32e25903f77df4
workflow-type: tm+mt
source-wordcount: '793'
ht-degree: 47%

---

# タスクレポートの作成

このビデオでは、以下について説明します。

* 複雑なフィルターを使用したタスクレポートの作成方法
* 作成するレポートの検索方法

>[!VIDEO](https://video.tv.adobe.com/v/335154/?quality=12&learn=on)

## アクティビティ 1：プロンプトを含むメモレポートを作成する

メモの内容、作成者、エントリ日、プロジェクト名、監査タイプに基づいて、ユーザーのメモ（コメントや更新など）またはシステムのメモを検索するために使用できるメモレポートを作成します。レポートに「Note Search」という名前を付けます。

メモテキストプロンプトを使用すると、このレポートは更新スレッド内を検索して、プロンプトで指定した基準を満たすスレッドを素早く抽出します。レポートを実行する際に、すべてのプロンプトに入力する必要はありません。必要なプロンプトはそれだけです。 空白の情報は自動的に無視されます。

ビューには、次の列を含める必要があります。

* メモ テキスト
* 監査テキスト
* エントリ日
* 所有者：名前
* 監査の種類
* タスク名
* 問題名

フィルタータブは空白のままにします。

プロジェクト名でグループ化します。

次のプロンプトを含めます。

* 監査テキスト
* メモ テキスト
* 所有者名
* エントリ日
* プロジェクト名
* 監査の種類

## アクティビティ 1 回答

1. **[!UICONTROL メインメニュー]**&#x200B;から&#x200B;**[!UICONTROL レポート]**&#x200B;を選択します。
1. **[!UICONTROL 新しいレポート]**&#x200B;メニューをクリックし、「**[!UICONTROL メモ]**」を選択します。
1. **[!UICONTROL 列（表示）]**&#x200B;で、以下を含む列を設定します。

   ![メモレポート列を作成する画面の画像](assets/note-report-columns.png)

   * [!UICONTROL メモ]／[!UICONTROL メモテキスト]
   * [!UICONTROL メモ]／[!UICONTROL 監査テキスト]
   * [!UICONTROL メモ]／[!UICONTROL エントリ日]
   * [!UICONTROL 所有者]／[!UICONTROL 名前]
   * [!UICONTROL メモ]／[!UICONTROL 監査タイプ]
   * [!UICONTROL タスク]／[!UICONTROL 名前]
   * [!UICONTROL イシュー]／[!UICONTROL 名前]

1. **[!UICONTROL エントリ日]**&#x200B;列を選択し、**[!UICONTROL 降順に並べ替え]**&#x200B;に変更します。
1. 「**[!UICONTROL グループ化]**」タブで、レポートを[!UICONTROL プロジェクト]／[!UICONTROL 名前]でグループ化するように設定します。

   ![メモレポートのグループ化を作成する画面の画像](assets/note-report-groupings.png)

1. [!UICONTROL フィルター]は空白のままにします。
1. 開く **[!UICONTROL レポート設定]** レポートに「Note Search」という名前を付けます。
1. Adobe Analytics の [!UICONTROL 説明] フィールドに、「選択した監査タイプと他のプロンプトに基づいて、システムまたはユーザーのメモを検索します。 「監査テキスト」列にはシステムのメモが表示され、「ユーザーのメモ」は「メモテキスト」列に表示されます。」

   ![メモレポート設定を作成する画面の画像](assets/note-report-report-options.png)

1. **[!UICONTROL 「詳細」タブ]**&#x200B;を選択し、レポートの読み込み時に表示されるようにします。
1. レポートがダッシュボードに含まれている場合、200 項目を表示するようにレポートを設定します。
1. 「**[!UICONTROL レポートプロンプト]**」をクリックし、以下を追加します。

   ![メモレポートプロンプトを作成する画面の画像](assets/note-report-report-prompts.png)

   * [!UICONTROL メモ]／[!UICONTROL 監査テキスト]
   * [!UICONTROL メモ]／[!UICONTROL メモテキスト]
   * [!UICONTROL 所有者]／[!UICONTROL 名前]
   * [!UICONTROL メモ]／[!UICONTROL エントリ日]
   * [!UICONTROL プロジェクト]／[!UICONTROL 名前]
   * [!UICONTROL メモ]／[!UICONTROL 監査タイプ]

1. 「**[!UICONTROL ダッシュボードにプロンプトを表示]**」チェックボックスをオンにします。
1. レポートを保存して閉じます。

## アクティビティ 2：管理チームのフィードバックレポートの作成

これは、システム管理者向けに作成されたフィードバックリクエストキューからのすべての問題を表示する問題レポートです。 このリクエストキューの作成方法については、 **システム管理者のフィードバックリクエストキューの作成** チュートリアル

このレポートは、カスタムフォームも使用します。 カスタムフォームの作成方法については、 [カスタムフォームの作成と共有](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/custom-data/custom-forms/custom-forms-creating-and-sharing-a-custom-form.html) チュートリアル

このカスタムフォームは、次のように作成する必要があります。

名前：管理者によるプロセスのフィードバック

1. プロセスのタイプ（ドロップダウンフィールド）
   * アクセスレベル
   * 承認プロセス（グローバルのみ）
   * 電子メール通知
   * レイアウトテンプレート
   * マイルストーンパス
   * プロジェクトテンプレート
   * リマインダー通知
   * リクエストキュー
1. プロセス名（1 行のテキストフィールド）
1. プロセスグレード（ドロップダウンフィールド）
   * 1 — 完全に無用
   * 2 — あまり役に立たない
   * 3 — 良いが良い
   * 4 — 優
1. 問題または良いニュース（段落テキストフィールド）

という名前の問題レポートを作成します。 **管理チームのフィードバックレポート**.

ビューには次の列が必要です。

* 問題：名前
* プライマリ連絡先：名前
* 問題：プロセスタイプ
* 問題：プロセス名
* 問題：プロセスグレード
* 問題または良いニュース
* 問題：入力日
* 問題：年齢
* 問題：割り当て
* 問題：ステータス

プロセスタイプでグループ化します。

フィードバックの問題が存在するリクエストキュープロジェクトの ID に基づいてフィルターします。


![管理者チームのフィードバックレポートのスクリーンショット](assets/create-a-system-admin-feedback-request-queue.png)



## アクティビティ 2 回答

1. **[!UICONTROL メインメニュー]**&#x200B;から&#x200B;**[!UICONTROL レポート]**&#x200B;を選択します。
1. 次をクリック： **[!UICONTROL 新しいレポート]** メニューと選択 **[!UICONTROL 問題]**.
1. **[!UICONTROL 列（表示）]**&#x200B;で、以下を含む列を設定します。

   ![問題レポート列を作成する画面の画像](assets/task-report-activity-2-1.png)

   * [!UICONTROL イシュー]／[!UICONTROL 名前]
   * [!UICONTROL プライマリ連絡先] > [!UICONTROL 名前] 注意：これは、列のラベルとして「Owner:Name」と表示されます。 詳細オプションをクリックし、 **カスタム列のラベル** フィールドに入力します。
   * [!UICONTROL 問題] > [!UICONTROL プロセスタイプ]
   * [!UICONTROL 問題] > [!UICONTROL プロセス名]
   * [!UICONTROL 問題] > [!UICONTROL プロセスグレード]
   * [!UICONTROL 問題] > [!UICONTROL 問題または良いニュース]
   * [!UICONTROL 問題] > [!UICONTROL 入力日]
   * [!UICONTROL 問題] > [!UICONTROL 年齢]
   * [!UICONTROL 問題] > [!UICONTROL 割当て]
   * [!UICONTROL 問題] > [!UICONTROL ステータス]

1. **[!UICONTROL エントリ日]**&#x200B;列を選択し、**[!UICONTROL 降順に並べ替え]**&#x200B;に変更します。
1. Adobe Analytics の **[!UICONTROL グループ化]** 」タブで、次の項目でグループ化するレポートを設定します。 **[!UICONTROL 問題] > [!UICONTROL プロセスタイプ]**.

   ![問題レポートのグループ化を作成する画面の画像](assets/task-report-activity-2-2.png)

1. Adobe Analytics の **[!UICONTROL フィルター]** 」タブで、 **[!UICONTROL 問題] > [!UICONTROL プロジェクト ID]** を追加します。

   ![問題のレポートフィルターを作成する画面の画像](assets/task-report-activity-2-3.png)

1. レポートを保存して閉じます。
