---
title: イシューのタイプと用語をカスタマイズする
description: 組織のニーズに合わせて、4 つのデフォルトのイシュータイプをカスタマイズし、名前を変更する方法を説明します。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10021
exl-id: d1e5c2d6-b001-4e9e-b72d-c792c70d09e8
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 100%

---

# イシューのタイプと用語をカスタマイズする

## デフォルトのイシュータイプの名前を変更する

[!DNL Workfront] には、ユーザーが作成するイシューの種類を分類するのに役立つ、4 種類のイシューが用意されています。 デフォルトは次のとおりです。

* [!UICONTROL バグレポート]
* [!UICONTROL 変更依頼]
* [!UICONTROL イシュー]
* [!UICONTROL リクエスト]

既存のイシュータイプが組織のイシュー管理のニーズに合わない場合や、組織が異なる用語を使用している場合はどうすればよいですか？

例えば、イシューを使用してプロジェクトのリスクを追跡するチームがあるとします。 システム管理者は、組織がバグレポートを追跡していないことを知っています。 したがって、使用されていないイシュータイプの名前（[!UICONTROL バグレポート]など）をプロジェクトのリスクに変更できます。

イシューのタイプはシステム全体のレベルで名前が変更されるので、変更はすべてのユーザーに適用されます。

1. **[!UICONTROL メインメニュー]**&#x200B;で「**[!UICONTROL 設定]**」をクリックします。
1. 左側のメニューパネルで「**[!UICONTROL プロジェクト環境設定]**」セクションを展開します。
1. 「**[!UICONTROL ステータス]**」を選択します。
1. 「**[!UICONTROL イシュー]**」タブを選択します。
1. 右上のメニューが[!UICONTROL システムステータス]に設定されていることを確認します。
1. リスト上部のイシュータイプの横にカーソルを合わせます。 鉛筆アイコンをクリックして、フィールド編集を有効にします。
1. イシュータイプの名前を変更します。
1. フィールドの外側をクリックして保存します。

![「設定」の[!UICONTROL ステータス]ページにある「イシュー」タブ](assets/admin-fund-issue-types.png)

>[!NOTE]
>
>これ以上のイシュータイプを作成したり、イシュータイプを削除することはできません。

<!---
learn more URLs
Customize default issue types
--->

## Workfrontの「イシュー」という用語を変更する

一部の組織では、計画外の作業アイテムを「イシュー」以外の用語で指します。 イシューはデフォルトの用語で、ソフトウェア全体（メニュー、レポート、フィールド名など）に表示されます。
Workfront の管理者は、レイアウトテンプレート機能を使用して、組織の用語に合わせてイシュー項目の名前を変更できます。 この新しい用語は、レイアウトテンプレートに割り当てられているユーザーに対して [!DNL Workfront] 全体に表示されます。

![[!UICONTROL イシュー]が強調表示された用語ウィンドウ](assets/admin-fund-issue-custom-terminology.png)

<!---
paragraph below needs a hyperlink
--->

システム管理者とグループ管理者がレイアウトテンプレートを作成する方法については、ラーニングパス、「新しい [!DNL Workfront] エクスペリエンスの管理者の基礎：第 3 部コントロールとインターフェイスのエクスペリエンス」を参照してください。

<!---
learn more URLs
Create and manage layout templates
--->
