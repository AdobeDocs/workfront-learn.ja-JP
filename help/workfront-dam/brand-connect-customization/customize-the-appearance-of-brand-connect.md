---
title: '[!UICONTROL Brand Connect] の外観のカスタマイズ'
description: '[!UICONTROL Workfront DAM] の [!UICONTROL Brand Connect] で、ナビゲーションバーとフッターをカスタマイズする方法、ホームページとログインページをカスタマイズする方法を説明します。'
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8980
exl-id: cf286347-46f0-4a7a-9f06-921975f28765
doc-type: video
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: ht
source-wordcount: '373'
ht-degree: 100%

---

# [!UICONTROL Brand Connect] の外観のカスタマイズ

このビデオでは、次の方法を学習します：

* ナビゲーションバーとフッターのカスタマイズ
* ホームページとログインページのカスタマイズ

>[!VIDEO](https://video.tv.adobe.com/v/335242/?quality=12&learn=on&enablevpops)

## その他の[!UICONTROL 外観]設定

[!UICONTROL 外観]メニューの[!UICONTROL フォント]オプションで、[!UICONTROL Brand Portal] 全体のすべてのテキストを選択したフォントでスタイルを設定します。800 種類を超える Google フォントがサポートされています。

![Brand Portal の[!UICONTROL 外観]メニュースタイルの[!UICONTROL フォント]オプション](assets/02-brand-connect-appearance-font.png)

## ホームページウィジェット

[!UICONTROL Brand Connect] ホームページのルック＆フィールを組織に合わせてカスタマイズします。ウィジェットを使用して、フォルダーや画像スライダーなどの要素を追加できます。組織に複数の [!UICONTROL Brand Connects] がある場合、それぞれにホームページを用意し、見た目を差別化することができます。

![[!UICONTROL Brand Connect] ホームページで利用可能なウィジェットのスクリーンショット](assets/03-brand-connect-home-page-widgets.png)

次のウィジェットを使用できます。

**A. カルーセル** - 画像スライダーに複数のアセットを表示します。各アセットに説明を追加できます。追加アイコンをクリックして、カルーセルに表示する画像を選択します。

**B. フォルダー** - 選択したアセットを含むフォルダーを表示します。追加アイコンをクリックして[!UICONTROL アセット選択]を開くと、フォルダーを選択できます。フォルダー内のアセットは、[!UICONTROL Brand Connect] ユーザーに表示されますが、許可されたユーザーのみがダウンロードできます。

**C. ライトボックス** - 既存の[!UICONTROL ライトボックス]を表示します。[!UICONTROL ライトボックス]内のアセットは、[!UICONTROL Brand Connect] ユーザーに表示されますが、許可されたユーザーのみがダウンロードできます。

**D. ブランドガイドライン** - 上部のナビゲーションバーの代わりに、または、上部のナビゲーションバーに加えて、ホームページにブランドガイドラインを表示します。

**E. 説明** - 短いテキストを表示する場合に使用します。

**F. 入力済み説明** - グレーの背景に表示するテキストコピーブロックを入力します。

**G. HTML** - HTML と CSS を使用してカスタムコンテンツを作成します。例えば、画像へのリンクを埋め込むことができます。[避けるべき HTML タグ](https://www.damsuccess.com/hc/en-us/articles/206170043-Brand-Connect-Admin-Guide#html)がいくつかあります。

## 検索バーの追加

組織の [!UICONTROL Brand Connect] のホームページをカスタムで設計する場合、ユーザーは[!UICONTROL アセット]エリアをクリックして検索を実行する必要があります。

ただし、システム管理者は HTML ウィジェットとこの HTML タグを使用して検索バーを作成できます。

&lt;webdambp.headersearch>&lt;/webdambp.headersearch>
