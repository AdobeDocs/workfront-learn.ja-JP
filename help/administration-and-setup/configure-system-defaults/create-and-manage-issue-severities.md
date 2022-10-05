---
title: 問題の重大度の作成と管理
description: 問題の重大度を設定および管理する方法について説明します。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
kt: 10020
exl-id: a5a9280b-0d48-413d-92de-f6a949e6b210
source-git-commit: 5d385de5cdcee0d433304c09507ba6bb5b0a10e6
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 3%

---

# 問題の重要度を作成および管理

## 問題の重要度の概要

重大度を使用して、問題の重大度や、実行中の作業に与える影響を示すことができます。

![[!UICONTROL 重大度] メニュー [!UICONTROL 問題の詳細] window](assets/admin-fund-severity-issue-details.png)

この [!UICONTROL 重大度] フィールドには、 [!UICONTROL 問題の詳細]. また、リストの列表示やカスタムレポートに含めることもできます。

[!DNL Workfront] には 5 つのデフォルトの重大度があります。

* [!UICONTROL 一時回避]
* [!UICONTROL 混乱を招く]
* [!UICONTROL 対処策のあるバグ]
* [!UICONTROL 対処策のないバグ]
* [!UICONTROL 致命的なエラー]

システム管理者は、必要に応じて、これらのデフォルトの重大度の名前を変更したり、新しい重大度を作成したりできます。

重大度は、 [!DNL Workfront].

## 問題の重要度を作成および管理

システム管理者は、必要に応じて新しい重大度を作成し、問題のワークフローを完了できます。

![[!UICONTROL 重大度] ページ内 [!UICONTROL 設定]](assets/admin-fund-severity-section.png)

1. クリック **[!UICONTROL 設定]** 内 **[!UICONTROL メインメニュー]**.
1. を展開します。 **[!UICONTROL プロジェクト環境設定]** 」セクションを使用して、
1. 選択 **[!UICONTROL 重大度]**.
1. クリック **[!UICONTROL 新しい重大度を追加]**.
1. 重大度に、目的に合った名前を付けます。
1. この **[!UICONTROL 重要度]** number は、問題の重大度に一致します。 最大の数は、最も大きい重大度に対応します。 この [!UICONTROL 重要度] 番号は一意である必要があります。
1. 優先度の色を選択します。 これは、グラフレポートや他の場所で [!DNL Workfront].
1. 重大度オプションの 1 つを **[!UICONTROL デフォルトの重大度]**. これは、Workfrontのすべての新しい問題に自動的に適用されます。
1. 重大度の説明（使用方法など）を含めます。
1. 保存するフィールドの外側をクリックします。

![[!UICONTROL 重大度] リスト](assets/admin-fund-severity-new.png)

### 重大度の変更

重大度が問題のワークフローに関連しなくなった場合は、名前の変更、非表示、削除が可能です。

重大度が不要になった場合は、 [!DNL Workfront] では、重大度を非表示にすることをお勧めします ( [!UICONTROL を隠す] 」ボックスをクリックします )。 これにより、問題のドロップダウンメニューから重大度が削除されますが、履歴データの重要度は保持されるので、レポートで引き続き使用できます。

![[!UICONTROL を隠す] 強調表示された列 [!UICONTROL 重大度] ページ内 [!UICONTROL 設定]](assets/admin-fund-severity-hide.png)

[!DNL Workfront] では、 **しない** 過去の問題で使用された重大度を削除します。 重大度を削除すると、別の重大度を置き換えるように求められます。 これにより、履歴データが変更され、レポートに影響を与える可能性があります。

![重大度ウィンドウを削除](assets/admin-fund-severity-delete.png)

<!---
learn more URLs
Create and customize issue severities
Update issue severity
--->
