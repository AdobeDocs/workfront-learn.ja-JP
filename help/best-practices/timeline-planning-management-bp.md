---
title: ベストプラクティス - タイムラインの計画と管理
description: Workfront でのプロジェクトタイムラインの設定、管理、および使用について、Adobe Workfront の専門家によるベストプラクティスのレコメンデーションを参照します。
feature: Get Started with Workfront
role: Admin, Leader, User
level: Beginner
jira: KT-10929
exl-id: 8c18746d-e23a-44d0-b1e3-ebf5ba8d022f
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1110'
ht-degree: 100%

---

# ベストプラクティス - タイムラインの計画と管理

## Adobe Workfrontの「ベストプラクティス」について

ベストプラクティスは、効果的で効率的な一連の行動を表すガイドラインです。お客様や会社のユーザーが簡単に採用でき、組織全体で正常に複製することができます。

これらのレコメンデーションを確認する際は、Workfront のベストプラクティスには普遍的なものもあれば、トピックに特化したものもあることにご留意ください。これらのベストプラクティスは、Workfront システムの設定や使用の指針となるフレームワークとしてご活用ください。

## このページのナビゲート

このページをスクロールすると、まずそのトピックに関するすべてのベストプラクティスの概要リストが表示されます。これにより、「理由」の詳細に踏み込むことなく、レコメンデーションを確認することができます。

「これらがベストプラクティスである理由」概要リストの後にあるエリアでは、ベストプラクティスの数例と、これがプロセスやツールなどとみなされる理由についてより詳細に説明しています。Workfront インスタンスでの実装を検討する必要があります。

</br>
</br>

## タイムラインの計画と管理のベストプラクティス

* 完了したすべてのプロジェクトには、完了したことを示すステータスが必要です。

* プロジェクトをコピーする場合は、新しいプロジェクトのステータスを「計画中」に設定します。

* ユーザーがタスクに費やした実際の時間を記録して、実際の時間と予定時間を比較できるようにします。

* 可能であれば、特定の開始日と完了日を選択するのではなく、タスクの期間と先行タスクを使用してプロジェクトタイムラインを構築およびアップデートします。

* 毎日（または設定されたスケジュールに従って毎週）、タスクのステータス、完了率（％）、実働時間を更新するようユーザーに依頼します。

* プロジェクト計画をアップデートするときにプロジェクトステータスを「計画中」に設定して、変更が行われたときに通知が自動的に送信されないようにします。

* プロジェクトで作業が割り当てられていないユーザーを、プロジェクトチームから削除します。

* 主に Workfront を使用してデータを表示するユーザーのために、左側のパネルメニューの上部にプロジェクト指標を配置します。


</br>
</br>


## これらがベストプラクティスである理由

**ベストプラクティス**

完了したすべてのプロジェクトには、完了したことを示すステータスが必要です。


**その理由は次のとおりです**

完了したすべてのプロジェクトが完了（または同等）のステータスを持っていることを確認することにより、Workfront インスタンスがクリーンで最新の状態に保たれます。プロジェクトのステータスを最新の状態に保ち、クローズすることで、ユーザーはどの作業がすでに完了しているかを簡単に知ることができるため、アクティブな優先事項に集中することができます。また、プロジェクト、タスク、リソースなどに関するレポート データが正確であることも保証します。


</br>
</br>

**ベストプラクティス**

プロジェクトをコピーする場合は、新しいプロジェクトのステータスを「計画中」に設定します。

**その理由は次のとおりです**

計画ステータス（または同等のステータス）は、プロジェクトの準備が整う前に、割り当て、タイムラインの変更などに関する Workfront 通知が送信されることを防ぎます。プロジェクトをコピーすると、プロジェクトオプションを含むダイアログボックスが表示されます。他のオプションを調整しつつ、ここでステータスを変更して、データが元のプロジェクトからコピーされたバージョンにコピーされないようにします。

</br>
</br>

**ベストプラクティス**

ユーザーがタスクに費やした実際の時間を記録して、実際の時間と予定時間を比較できるようにします。


**その理由は次のとおりです**

タスクの作業時間を把握することにより、将来のプロジェクトを計画する際に、プロジェクトテンプレートをアップデートして精度を高めることができます。また、Workfront のリソース管理ツールを使用したリソースの見積もりが、より正確であることも意味します。

</br>
</br>

**ベストプラクティス**

可能であれば、特定の開始日と完了日を選択するのではなく、タスクの期間と先行タスクを使用してプロジェクトタイムラインを構築およびアップデートします。

**その理由は次のとおりです**

期間と先行タスクを柔軟なタスクの制約（できるだけ早く／できるだけ遅く）と組み合わせて使用することにより、プロジェクト計画を通じて「重ねて表示（カスケード）」するタイムラインの日付を自動的に変更できます。例えばあるタスクの期間が 1 日長くなると、そのタスクの予定完了日に加え、次のタスクの完了日も変更されます。

タスクの特定の開始日と完了日を選択すると、タスクの制約が日付を「ロック」するもの（必須開始日、必須完了日、固定日付）に変更されます。つまり、タイムラインの日付を手動でアップデートする必要があります。

</br>
</br>


**ベストプラクティス**

毎日（または設定されたスケジュールに従って毎週）、タスクのステータス、完了率（％）、実働時間を更新するようユーザーに依頼します。

**その理由は次のとおりです**

Workfront のレポートの制度は、Workfront で入力されたデータと同程度です。ステータスや完了率などの作業の進捗状況を示す情報が定期的に更新されていないと、作業の進捗状況を示すレポートは正確ではなくなります。毎日更新することで、リアルタイムレポートデータの精度を最大限に高めることができます。


タスクのステータスは、以前の作業が完了し、新しいタスクを開始できる時期をユーザーに知らせるためにも使用されます。作業アイテムの実際の進行状況を反映するようにタスクステータスが変更されない場合、Workfront は適切な通知を送信することができません。

</br>
</br>

**ベストプラクティス**

プロジェクト計画をアップデートするときにプロジェクトステータスを「計画中」に設定して、変更が行われたときに通知が自動的に送信されないようにします。

**その理由は次のとおりです**

プロジェクト計画が変更されると、タスクの割り当て、開始予定日や完了予定日、およびその他の設定も変更されるため、通知が複数生成される場合があります。これはユーザーの混乱を招き、適切な割り当てや締め切りなどが分かりにくくなってしまう可能性があります。

「計画中」ステータスは、プロジェクト計画がまだ開発中であるか、プロジェクトがまだ稼動する準備ができていないため、プロジェクトチームのメンバー（タスクやイシューを割り当てられたユーザー、またはプロジェクトへのアクセス権を持つ他のユーザー）にプロジェクトに関する通知を送信しないよう Workfront に指示します。変更が完了したら、プロジェクトのステータスを現在に戻すと、通知が送信されます。このプロセスに従うと、ユーザーが受信する通知の量を最小限に抑えることができます。

</br>
</br>

**ベストプラクティス**

プロジェクトで作業が割り当てられていないユーザーを、プロジェクトチームから削除します。


**その理由は次のとおりです**

プロジェクトのタスクまたは問題を誰かに割り当てると、そのユーザーは、プロジェクトのスケジュールセクションとユーザーセクションのプロジェクトチームリストに追加されます。ただし、ユーザーを割り当てから削除しても、プロジェクトチームリストには残ります。これは、プロジェクトチームの一員としてユーザーがプロジェクトのアクティビティに関する通知を受け取り、自分が参加しているプロジェクトリストにプロジェクトが表示されるため、混乱を招く可能性があります。


さらにプロジェクトチームメンバーは、プロジェクトとそのタスク、イシュー、およびドキュメントに対する権限を取得します。これにより、ユーザーが必要のない、または持つべきではない Workfront のアイテムにアクセスできるようになる可能性があります。

</br>
</br>

**ベストプラクティス**

主に Workfront を使用してデータを表示するユーザーのために、左側のパネルメニューの上部にプロジェクト指標を配置します。

**その理由は次のとおりです**

プロジェクトを管理したり、タスクの割り当てを実行したりしないほとんどのリーダー、エグゼクティブ、およびその他のユーザーは、最初にプロジェクトを開いたときに、このレベルのプロジェクト指標を確認することができることに感謝するでしょう。レイアウトテンプレートを使用して、プロジェクト指標をプロジェクトページの左のパネルメニューの一番上に移動し、ユーザーが見やすく、またアクセスしやすくします。
