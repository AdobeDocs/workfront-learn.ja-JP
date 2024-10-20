---
title: ベストプラクティス - テキストモードのレポート
description: Workfront テキストモードのレポートの設定、管理、使用に関する、Adobe Workfront のエキスパートによるベストプラクティスのレコメンデーションについて説明します。
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
jira: KT-10928
exl-id: c624545c-ba42-4cc3-aafe-8be15baadb75
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 100%

---

# ベストプラクティス - テキストモードのレポート

## Adobe Workfrontの「ベストプラクティス」について

ベストプラクティスは、効果的で効率的な一連の行動を表すガイドラインです。お客様や会社のユーザーが簡単に採用でき、組織全体で正常に複製することができます。

これらのレコメンデーションを確認する際は、Workfront のベストプラクティスには普遍的なものもあれば、トピックに特化したものもあることにご留意ください。これらのベストプラクティスは、Workfront システムの設定や使用の指針となるフレームワークとしてご活用ください。

## このページのナビゲート

このページをスクロールすると、まずそのトピックに関するすべてのベストプラクティスの概要リストが表示されます。これにより、「理由」の詳細に踏み込むことなく、レコメンデーションを確認することができます。

「これらがベストプラクティスである理由」概要リストの後にあるエリアでは、ベストプラクティスの数例と、これがプロセスやツールなどとみなされる理由についてより詳細に説明しています。Workfront インスタンスでの実装を検討する必要があります。

</br>
</br>

## テキストモードのレポートのベストプラクティス

* 可能な限り、リストレポート列で、計算カスタムフィールドの代わりに、テキストモードの値の式を使用します。

* レポートの説明に、テキストモードの計算で使用する計算を配置します。

</br>
</br>

## これらがベストプラクティスである理由

**ベストプラクティス**

可能な限り、リストレポート列で、計算カスタムフィールドの代わりに、テキストモードの値の式を使用します。



**その理由は次のとおりです**

テキストモードの値の式は、レポートの実行時に計算され、レポートが更新されるたびに再計算されます。つまり、常に最新のデータと正確なレポートを入手できます。



（カスタムフォームで使用する）計算カスタムフィールドは、データが Workfront に表示される場合、自動的に更新されません。代わりに、Workfront に保存されている最新の計算結果が表示されます。つまり、これらの値がいつでも「古い」または有効期限切れになる可能性があります。計算カスタムフィールドでは、式を再計算するか、計算されたフィールドを含むオブジェクトを編集して保存することで、手動で更新する必要があります。これには時間がかかるだけでなく、忘れやすいというな側面もあります。


</br>
</br>

**ベストプラクティス**

レポートの説明に、テキストモードの計算で使用する計算を配置します。



**その理由は次のとおりです**

レポートの説明にテキストモードの計算を含めると、計算がどのように作成されたのか、どのような情報を表示する必要があるかを他のユーザーが理解するのに役立ちます。また、将来更新が必要になった場合に備えて、レポートがどのように作成されたかをシステム管理者に通知します。
