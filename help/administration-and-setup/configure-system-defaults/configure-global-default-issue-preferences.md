---
title: グローバルなデフォルトの問題設定を構成
description: 変換された問題の問題の環境設定、実際の日付、問題へのアクセスを設定する方法について説明します。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
kt: 10018
exl-id: 9924e479-c300-47b4-8e40-241ebb2435cf
source-git-commit: 3ded3fe9d8b97b1c11cb382f8088930842399c98
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 0%

---

# グローバルなデフォルトの問題設定を構成

システム全体のいくつかの設定では、 [!DNL Workfront].

ベストプラクティスは、グローバルなデフォルトをそのままにし、プロジェクトマネージャが必要な調整をプロジェクトレベルまたはプロジェクトテンプレートで行えるようにすることです。

グローバルな問題の環境設定は調整できますが、ユーザーと [!DNL Workfront] コンサルタントは、組織のワークフロー、プロセス、レポートニーズに必要な設定について説明します。 また、特定の設定が変更された場合の動作を把握するのに、担当のコンサルタントにお手伝いをします。

問題の環境設定を使用すると、問題がタスクやプロジェクトに変換される際のオプション、実際の日付の計算方法、問題が割り当てられた際のプロジェクトアクセス権を取得するユーザーを制御できます。 これらの設定が [!DNL Workfront].

## 変換された問題の環境設定

これらの設定は、 [!DNL Workfront].

![[!UICONTROL タスクと問題] 環境設定ウィンドウ [!UICONTROL 問題] 強調表示されたセクション](assets/admin-fund-issue-prefs-converting.png)

1. クリック **[!UICONTROL 設定]** 内 **[!UICONTROL メインメニュー]**.
1. を展開します。 **[!UICONTROL プロジェクト環境設定]** 」セクションを使用して、
1. 選択 **[!UICONTROL タスクと問題]**.
1. スクロールして **[!UICONTROL 問題]** 」セクションに入力します。
1. 目的のオプションをクリックします。
1. 完了したら保存します。

組織に適したオプションを選択できるよう、この節のオプションについて説明します。

* **[!UICONTROL 解決可能な問題のステータスを、解決オブジェクトのステータスが変更されたときに自動的に更新します]**

   この設定では、元の問題の解決と、新しいオブジェクト（タスクまたはプロジェクト）の解決を関連付けることができます。

   この設定を有効（オン）にすると、タスクまたはプロジェクトのステータスと同じステータスキーを持つカスタムイシューステータスを作成できます。 タスクまたはプロジェクト（解決可能なオブジェクト）がカスタムステータスに設定されている場合、変更は問題ステータスにも表示されます。

   無効にすると、解決オブジェクトのステータスは、カスタムのステータスではなく、自動的にデフォルトのステータスに設定されます。

   この設定を有効にするには、[!UICONTROL 元の問題を保持し、その解決をタスクに結び付けます]」オプションを選択する必要があります。

* **[!UICONTROL 元の問題を保持し、タスク/プロジェクトに対する解決策を維持]**

   問題が変換されると、次の情報が表示されます [!DNL Workfront] 元の問題を保持する。 タスクまたはプロジェクトのステータスが変更されると、イシューのステータスが変わります。 タスクまたはプロジェクトが完了とマークされると、問題は解決済みとマークされます。

   このオプションを選択しない場合、元のイシューは削除され、変換されたタスクまたはプロジェクトのみが残ります。

   この設定は、プロジェクトで最初にログオンした問題や、 [!DNL Workfront] リクエストキュー。

* **[!UICONTROL プライマリの連絡先がタスク/プロジェクトにアクセスできるようにする]**

   これにより、元のイシューを作成したユーザーは、変換処理の実行時に作成されたタスクまたはプロジェクトにアクセスできます。 作業内容を確認し、更新を行い、進捗を常に知らせることができます。

* **[!UICONTROL 変換中にこれから設定が変更できるようにする]**

   このオプションを選択すると、「[!UICONTROL 元の問題を保持]&quot;および&quot;[!UICONTROL プライマリ連絡先を許可]」は、ユーザーが問題を変換することで変更できます。 デフォルトを変更しない場合は、このオプションの選択を解除します。

<!---
learn more URLs
Configure system-wide task and issue preferences
Issue statuses
Create and customize system-wide statuses
--->

## 実際の日付設定

全体で複数のタイプの日付が使用されます [!DNL Workfront]. 実際の日付は、 [!DNL Workfront] 特定のステータスが変更された場合にが生成されます。

この [!UICONTROL 実際の開始日] タイムスタンプは、問題のステータスが「新規」から「別の」に変わったときに作成されます。 この [!UICONTROL 実際の完了日] タイムスタンプは、問題のステータスが閉じられたことを示すステータスに変わったときです。

この環境設定では、タスクとタスクの両方の実際の日付設定が制御されることに注意してください。

![[!UICONTROL タスクと問題] 環境設定ウィンドウ [!UICONTROL 実際の日付] 強調表示されたセクション](assets/admin-fund-issue-prefs-actual-dates.png)

1. クリック **[!UICONTROL 設定]** 内 **[!UICONTROL メインメニュー]**.
1. を展開します。 **[!UICONTROL プロジェクト環境設定]** 」セクションを使用して、
1. 選択 **[!UICONTROL タスクと問題]**.
1. スクロールして **[!UICONTROL 実際の日付]** 」セクションに入力します。
1. 目的のオプションを **[!UICONTROL 実際の開始日]** — [!UICONTROL 今すぐ] （現在の日時）または [!UICONTROL 計画開始日] ( [!UICONTROL 実際の開始日] は、問題の詳細で設定された開始日に一致します )。
1. 次に、 **[!UICONTROL 実際の完了日]** — [!UICONTROL 今すぐ] （現在の日時）または [!UICONTROL 計画完了日] ( [!UICONTROL 実際の開始日] は、問題の詳細で設定された日付に一致します )。
1. 完了したら保存します。


<!---
learn more URLs
Definitions for the project, task, and issue dates within Workfront
Configure system-wide task and issue preferences
--->

## アクセスの問題

この [!UICONTROL アクセス] 問題の設定は、Workfrontで問題を割り当てたときにユーザーに付与されるアクセスを制御します。 これらの設定は、問題が関連付けられているプロジェクトへのアクセスに加えて、問題自体へのアクセスを制御します。

これらの設定を変更する前に、ワークフローやプロセスのニーズについて、 [!DNL Workfront] コンサルタントと社内ガバナンスチーム。

![[!UICONTROL タスクと問題] 環境設定ウィンドウ [!UICONTROL 誰かが問題に割り当てられたとき] 強調表示されたセクション](assets/admin-fund-issue-prefs-access-1.png)

1. クリック **[!UICONTROL 設定]** 内 **[!UICONTROL メインメニュー]**.
1. を展開します。 **[!UICONTROL プロジェクト環境設定]** 」セクションを使用して、
1. 選択 **[!UICONTROL タスクと問題]**.
1. スクロールして **[!UICONTROL アクセス]** 」セクションで、[!UICONTROL 誰かが問題に割り当てられたとき]&quot;オプション。
1. イシュー自体の共有アクセスを設定します — [!UICONTROL 表示], [!UICONTROL 投稿]または [!UICONTROL 管理]. [!DNL Workfront] では、詳細設定オプションをそのまま残すことをお勧めします。
1. 問題の担当者がプロジェクトへのアクセス権も持っている場合は、「 」チェックボックスをオンにします
1. 次に、プロジェクトの共有アクセス権を選択します — [!UICONTROL 表示], [!UICONTROL 投稿]または [!UICONTROL 管理]. 設定時に、 [!UICONTROL 詳細オプション]を使用する場合は、組織のワークフローとアクセスニーズに注意してください。
1. 完了したら保存します。

![[!UICONTROL アクセス] ウィンドウ表示 [!UICONTROL 投稿] options](assets/admin-fund-issue-prefs-access-2.png)

<!---
learn more URLs
Configure system-wide task and issue preferences
Grant access to issues
--->
