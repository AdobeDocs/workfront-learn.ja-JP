---
title: 既存の Adobe Workfront インスタンスの管理
description: 新規システムまたはグループ管理者として Workfront のインスタンスを評価、把握および最適化するためのキーフレーズについて説明します。
feature: System Setup and Administration
type: Tutorial
role: Admin
level: Beginner,Intermediate,Experienced
activity: use
jira: KT-11747
team: Technical Marketing
thumbnail: null
exl-id: ad900f59-319b-49ee-bc23-e816edc2de24
source-git-commit: be1afb2a1c24b35c7fc84e77fab08934e3cbbe48
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 66%

---

# 既存の Adobe Workfront インスタンスの管理

Workfront の優れた点として、カスタマイズ可能なことがあります。Workfront の難しい点として、カスタマイズ可能なことがあります。既存の Workfront インスタンスを引き継ぐ新規システム（またはグループ）管理者であれば、それが元々どのように構成され、設定されていたかを把握するのは大変なことでしょう。

しかし、継承されたインスタンスのチェックリストを使用すると、お使いのインスタンスについて知る必要があるすべてのことを学ぶことができます。

![継承されたインスタンスのチェックリストの画像](assets/wf-inherited-instance-image.png)
<br></br>

継承インスタンスのチェックリストで、質問、リソース、リンクの包括的なセットを確認して、その設定方法を明確に理解します。

このチェックリストは、Workfrontブループリントとして、またダウンロード可能な Excel スプレッドシートとして作成されています。 ブループリントを使用して、Workfrontで作業を管理し、ドキュメント化することをお勧めします。

ブループリントとスプレッドシートは、タイムラインではなくトピック別に整理されているので、自分と組織にとって最適な方法で進めることができます。. 提供される期間は一例に過ぎません。具体的なニーズに合わせて調整する必要があります。 1 回で全てを行う必要はありません！

可能な限り、組織内の他のユーザーと協力して、これらの要素を確認および文書化し、大きな変更がある場合はドキュメントを最新の状態に保つことをお勧めします。 インスタンスの将来の管理者にとって、非常に有用なものになるはずです。

* ブループリントをダウンロードするには、独自のWorkfrontインスタンスのメインメニューに移動し、「ブループリント」を選択します。 「Inherited Instance Basics」というタイトルのブループリントを見つけます。 「|チェックリスト」をクリックし、「インストール」をクリックします。 実稼動環境またはサンドボックス環境を選択し、引き続き設定します。 ブループリントのインストールと設定について詳しくは、 [ここ](https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/blueprints/blueprints-install.html?lang=en).

* Excel チェックリストをダウンロードするには、 [ここ](assets/adobe-workfront-system-admin-playbook-inherited-instance.xlsx).

ブループリントや Excel チェックリストを使用する場合でも、このプロセスは、検出、監査、ドキュメントという 3 つの主要なフェーズで考えることができます。 以下に説明と理想的な結果を示します。

<br>
</br>

## フェーズ 1：学習と探索

<b>推奨期間：4 週間</b>

まず最初にすべきことは、Workfront のインスタンスが、現在、どのように設定されているかを把握することです。

これには、関係者へのインタビューを実施したり既存のドキュメントを確認したりして、組織内の様々なグループが Workfront をどのように活用しているかを把握することが含まれます。

技術的な観点から Workfront に精通していない場合は、システム管理者トレーニングを受講してください。このトレーニングでは、様々な設定がどのように Workfront の各ツール（そして潜在的に各ユーザー）で機能し、影響するかについて、必要なインサイトを得ることができます。

このフェーズが終了するまでに、以下を得る必要があります。

* 組織で Workfront を使用する理由の明確な理解

* 主要なユースケースを含む、お使いのインスタンスの健全性に関する一般的な感覚

* うまくいっていることや、プロセスとユーザーニーズの間にある課題やギャップを概説したドキュメント
<br>
</br>

## フェーズ 2：システム監査

<b>推奨期間：4 週間 </b>

最初の探索の後で、インスタンスのより技術的な監査を実行することをお勧めします。つまり、現在の設定と構成がビジネス要件およびニーズを確実に満たすようにするために必要になる可能性のある、変更や機能強化を決定する必要があります。

このフェーズが終了するまでに、以下を得る必要があります。

* インスタンスの現在の状態のより深い見識

* ビジネスニーズに対応するために、インスタンスに加えたい変更や機能強化の特定
<br>
</br>

## フェーズ 3：ドキュメント化と最適化

<b>推奨期間：2 週間（以後、継続的に更新） </b>

フェーズ 1 と 2 で学んだことに基づいて、インスタンスのドキュメントを作成または更新し、戦略的課題やプログラムレベルの課題に対処するためのロードマップを策定します。

このフェーズが進行中の間、以下を得る必要があります。

* このドキュメントの各タブにわたる質問に答える、一元化されたドキュメントの作成

* 最優先のワークフロー、自動化、統合の図表

* 組織的課題や戦略的課題を改善するための将来の機能強化をドキュメント化したバックログまたはロードマップ

<br>
各フェーズを経ることで、また、継承されたインスタンスのチェックリストを活用することで、新規システムまたはグループ管理者として、Workfront インスタンスがどのように構成されているか、どのような調整や機能強化を行う必要があるかをより深く把握し、組織の Workfront エクスペリエンスを最適化するためのドキュメントを固めることができます。

<br>
</br>

追加情報については、以下を参照してください。
* [ウェビナー：継承されたインスタンスを引き継ぐためのヒント](https://experienceleaguecommunities.adobe.com/t5/workfront-discussions/webinar-system-admin-essentials-tips-for-taking-over-an-existing/td-p/571873)
* [Workfront 実装の目標の定義](https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/get-started-administration/define-wf-goals-objectives.html?lang=ja)
* [ブログ投稿：エグゼクティブスポンサーシップとリーダーシップへの価値](https://experienceleaguecommunities.adobe.com/t5/workfront-blogs/customer-success-tips-executive-sponsorship-and-value-to/ba-p/518353)
* [ブログ投稿：Adobe Workfront KPI の概要](https://experienceleaguecommunities.adobe.com/t5/workfront-blogs/kpi-dashboards-in-the-new-workfront-experience-introduction-to/ba-p/549001)
