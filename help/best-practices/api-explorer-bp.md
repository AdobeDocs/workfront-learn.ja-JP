---
title: ベストプラクティス — API エクスプローラー
description: Workfrontの API エクスプローラーの設定、管理、使用に関するAdobe Workfrontの専門家によるベストプラクティスの推奨事項を確認します。
feature: Workfront API
role: Admin, Leader, User
level: Beginner
kt: 10902
exl-id: 0f3fc5ba-d01a-4337-829f-def0830ddf81
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# ベストプラクティス — API エクスプローラー

## Adobe Workfrontの「ベストプラクティス」とは

ベストプラクティスは、効果的で効率的な行動方針を示すガイドラインです。は、お客様やお客様の会社のユーザーに簡単に採用されます。とは、組織全体で正常にレプリケートできます。

これらの推奨事項を確認する際は、Workfrontのベストプラクティスの中には普遍的なものと、トピックに特化したものがあるものもあることに注意してください。 これらのベストプラクティスをフレームワークとして使用し、Workfrontのシステムの設定と使用をガイドします。

## このページの移動

このページをスクロールすると、まずそのトピックに関するすべてのベストプラクティスの概要リストが表示されます。 これにより、「理由」の詳細を調べることなく、レコメンデーションを確認できます。

「これらのベストプラクティスはなぜですか？」 領域の概要リストの後に、ベストプラクティスの一部、およびプロセスやツールと見なされる理由について詳しく説明しています。Workfrontインスタンスを使用した実装を検討してください。

</br>
</br>

## API Explorer のベストプラクティス

* サードパーティシステムからの統合で使用されるカスタムフィールドの命名規則を確立します。

* Workfrontプロジェクトを使用した統合で使用されるすべてのカスタムフィールドを追跡します。

* システム管理者が使用するレポートに、オブジェクト ID フィールドを追加します。

</br>
</br>

## これらのベストプラクティスはなぜですか？

**ベストプラクティス**

サードパーティシステムからの統合で使用されるカスタムフィールドの命名規則を確立します。

**その理由は次のとおりです。**

カスタムフォームを作成するすべてのユーザーは、命名規則を把握していることを確認します。その結果、統合用に予約されたフィールドを誤って使用することはなくなります。 統合とワークフローに応じて、同じフィールドを複数の方法で使用すると、データが変更または上書きされ、レポートに誤ったデータが表示される場合があります。

</br>
</br>


**ベストプラクティス**

Workfrontプロジェクトを使用した統合で使用されるすべてのカスタムフィールドを追跡します。

**その理由は次のとおりです。**

プロジェクトは、カスタムフィールド名や、カスタムフィールド名との統合などをログに記録するのに最適な場所です。 これにより、重複したカスタムフィールドを作成したり、同じカスタムフィールドを複数の統合で使用したりするのを防ぐのに役立ちます。

</br>
</br>


**ベストプラクティス**

システム管理者が使用するレポートに、オブジェクト ID フィールドを追加します。

**その理由は次のとおりです。**

システム管理者は、API や他の統合を使用する際に、多くの場合、ID 番号でWorkfrontのオブジェクトを参照する必要があります。 作業対象のオブジェクト（プロジェクト、タスク、タスク、イシュー、テンプレート、カスタムフォームなど）のビューに ID フィールドを含めます。 アクセスやコピーを容易にする。
