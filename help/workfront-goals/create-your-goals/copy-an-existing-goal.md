---
title: 既存の目標のコピー
description: での既存の目標のコピー方法を説明します。 [!DNL Workfront Goals].
activity: use
team: Technical Marketing
feature: Workfront Goals
type: Tutorial
role: User
level: Beginner
kt: 10121
exl-id: bf9ac10a-8419-458b-b4e8-bedb0ad3b98f
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 0%

---

# 既存の目標のコピー

四半期の終わりで、次の期間の既存の目標を再作成するとします。 または、目標を達成していないので、次の期間に延長する必要がある可能性があります。 その目標を作成する最善の方法は何ですか？ 既存の目標をコピーして変更します。

複数のチームメンバーが同じ目標を持ち、それぞれに対して 1 つの目標を作成する必要がある場合も、既存の目標をコピーすると便利です。

<!--
Pro-tips graphic
-->

目標をコピーする前に考慮すべき点を次に示します。

* 目標期間を除き、元の目標からのすべての情報がコピーされます（過去の情報であるため）。
* 既存の目標の結果をコピーして、新しい目標に転送できます。
* コピーした結果は、デフォルトで同じ所有者に割り当てられます。
* 既存の目標の進行状況を新しい目標にコピーすることはできません。
* 目標をコピーする際に、目標のアクティビティをコピーすることはできません。

## 目標のコピー方法

1. 目標名をクリックして、 **[!UICONTROL 目標の詳細]** パネル。
1. 3 ドットアイコンをクリックし、「 **[!UICONTROL コピー]**.
1. コピーした目標に関する次の情報を更新します。
   * **新しい目標** — これは、新しい目標の名前です。 デフォルトは、元の目標の名前です。
   * **期間** — 目標を達成する期間。 ドロップダウンメニューから期間を選択するか、「カスタム日付の定義」をクリックしてカスタム期間を示します。 デフォルトの期間は常に現在の四半期です。
   * **所有者** — 目標の所有者。 ユーザー、チーム、グループ、会社のいずれかを指定できます。 デフォルトは、元の目標の所有者です。
   * **説明** — 目標に関する追加情報。

1. 次を確認します。 **[!UICONTROL 結果をコピー]** 」ボックスに移動します。 コピーしたゴールの結果には、元のゴールの結果と同じ所有者、名前、測定値が含まれます。

1. 「**[!UICONTROL 保存]**」をクリックします。コピーした目標は、ステータスが「ドラフト」で保存されます。

   ![画像 [!UICONTROL 目標の詳細] パネル内 [!DNL Workfront Goals] と [!UICONTROL コピー] オプション](assets/03-workfront-goals-copy-a-goal.png)

1. クリック **[!UICONTROL 有効化]**：目標のステータスを「アクティブ」に更新します。 目標を「アクティブ化」するには、目標にアクティビティが関連付けられている必要があります。

1. 次をクリック： **X** の右上に [!UICONTROL 目標の詳細] パネルを使用して閉じます。

前の期間に完了していない目標をコピーし、次の期間にその目標を引き続き使用する場合は、次の手順を実行します。

1. 元の目標 ( **[!UICONTROL 目標リスト]**, **[!UICONTROL チェックイン]** セクションまたは **[!UICONTROL パルス]** 」セクションに入力します。
1. 目標に対してコメントを付け、目標がコピーされ、より新しい目標が作成されたことを示します。
1. 元の目標を閉じて、元の期間の進行状況を保持します。 「 **[!UICONTROL 目標の詳細]** パネルと選択 **[!UICONTROL 閉じる]** を選択します。
1. を更新します。 [!UICONTROL 初期] 新しい結果の値を **[!UICONTROL ターゲット]** の値が前の結果の値になるので、新しい目標の進捗状況は前の期間に達した時点から計算を開始します。
