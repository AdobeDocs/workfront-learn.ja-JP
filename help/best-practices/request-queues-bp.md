---
title: ベストプラクティス - リクエストキュー
description: Workfront リクエストキューの設定、管理、使用に関する、Adobe Workfront のエキスパートによるベストプラクティスのレコメンデーションについて説明します。
feature: Resource Management
role: Admin, Leader, User
level: Beginner
jira: KT-10921
exl-id: dbb961f9-c207-49f1-9545-ec127f983c15
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1482'
ht-degree: 100%

---

# ベストプラクティス - リクエストキュー

## Adobe Workfrontの「ベストプラクティス」について

ベストプラクティスは、効果的で効率的な一連の行動を表すガイドラインです。お客様や会社のユーザーが簡単に採用でき、組織全体で正常に複製することができます。

これらのレコメンデーションを確認する際は、Workfront のベストプラクティスには普遍的なものもあれば、トピックに特化したものもあることにご留意ください。これらのベストプラクティスは、Workfront システムの設定や使用の指針となるフレームワークとしてご活用ください。

## このページのナビゲート

このページをスクロールすると、まずそのトピックに関するすべてのベストプラクティスの概要リストが表示されます。これにより、「理由」の詳細に踏み込むことなく、レコメンデーションを確認することができます。

「これらがベストプラクティスである理由」概要リストの後にあるエリアでは、ベストプラクティスの数例と、これがプロセスやツールなどとみなされる理由についてより詳細に説明しています。Workfront インスタンスでの実装を検討する必要があります。

</br>
</br>

## リクエストキューのベストプラクティス

* リクエストキューの各要素（リクエストキュープロジェクト、トピックグループ、キューのトピック、ルーティングルール）の説明を含めます。

* 「リクエストキュー」または「運用中」と呼ばれるプロジェクトステータスを作成し、「現在」と同じ値を使用して、リクエストキュープロジェクトを他のプロジェクトと区別します。

* キューを通じて送信されたリクエストに対してイシューの承認を使用するプランがある場合は、却下というイシューステータスを作成します。

* リクエストキューに「ユニバーサル」カスタムフォームを割り当てて、企業全体で一貫したデータをできるだけ多く取り込みます。

* リクエストキューを「全員」と共有しないようにします。キューの詳細設定を設定して、ユーザーのニーズに関連するキューのみが表示されるようにします。

* トラフィック管理者、システム管理者、割り当てられたユーザーがイシューに直接取り組むことができるように、リクエストキューレポートを含むダッシュボードを作成して割り当てます。

* レイアウトテンプレートを使用して、キューを作成する必要のないユーザー向けに、プロジェクトの左側のパネルメニューからリクエストキューの設定オプションを削除します。

* ユーザーが Workfront 関連の質問をしたり、システムの設定に関するリクエストを作成したり、新しいユーザーのトレーニングをスケジュールしたりできるように、システム管理者のリクエストキューを作成します。

* リクエストキューを定期的に監査して、使用されていないキューを識別し、共有しないようにします。

* トピックグループを使用して、リクエストキュー内の 10 個を超えるキューのトピックを整理し、短くて管理しやすいリストを作成します。

* 複数のキューを作成するのではなく、トピックグループとキューのトピックを使用してリクエストキューを分割することで、ユーザーが使用できるリクエストキューの合計数を制御します。

* 各キューのトピックのルーティングルールを設定します。少なくとも、デフォルトのルーティングルールは設定します。

* 選択的なルーティングが必要な場合は、トピックグループとキューのトピックを活用します。

* 個人ではなくチームにリクエストをルーティングします。


</br>
</br>


## これらがベストプラクティスである理由


**ベストプラクティス**

リクエストキューの各要素（リクエストキュープロジェクト、トピックグループ、キューのトピック、ルーティングルール）の説明を含めます。

**その理由は次のとおりです**

説明により、グループ管理者、今後のシステム管理者、リクエストキューを保持する他のユーザーは、リクエストキューの各部分で何が行われるかを正確に把握できます。

また、説明情報は、新規リクエストウィンドウのフィールドの情報アイコンにポインタを合わせた際にも表示されます。

説明は長くする必要はありません。要素の目的や使用に関する簡単なコメントだけにします。

</br>
</br>

**ベストプラクティス**

「リクエストキュー」または「運用中」と呼ばれるプロジェクトステータスを作成し、「現在」と同じ値を使用して、リクエストキュープロジェクトを他のプロジェクトと区別します。

**その理由は次のとおりです**

リクエストキューは、プロジェクト内で「ライブ」になっているので、キューをアクティブにするには、現在と等しいステータスにする必要があります。

「現在」ステータスの実際の作業プロジェクトとリクエストを区別するために、「リクエストキュー」または「運用中」と呼ばれるリクエストキューでのみ使用されるステータスを作成します。その後、このステータスを使用して、レポートの作成中にリクエストキュープロジェクトを除外したり含めたりできます。

</br>
</br>

**ベストプラクティス**

イシュー承認を使用する場合は「却下」というイシューステータスを作成し、「却下の場合」オプションを「却下」ステータスに設定します。

**その理由は次のとおりです**

「却下」ステータスを使用すると、リクエストがレビューおよび却下されたことが明確になります。

</br>
</br>

**ベストプラクティス**

リクエストキューに「ユニバーサル」カスタムフォームを割り当てて、企業全体で一貫したデータをできるだけ多く取り込みます。

**その理由は次のとおりです**

「ユニバーサル」カスタムフォームは、送信するリクエストのタイプに関係なく、リクエストに必要な標準情報を収集します。

「ユニバーサル」カスタムフォームを使用すると、作成し維持する必要のあるカスタムフォームの数を減らすことができます。 また、すべてのリクエストが同じ方法で同じ情報を収集するので、一貫したレポートとデータ分析が可能になります。

</br>
</br>

**ベストプラクティス**

リクエストキューを「全員」と共有しないようにします。キューの詳細設定を設定して、ユーザーのニーズに関連するキューのみが表示されるようにします。

**その理由は次のとおりです**

ほとんどの場合、リクエストキューは、チーム、ベンダー、顧客などの特定の人々とのみ共有する必要があります。リクエスタがリクエストキューリストで必要なものだけを参照すると、見つけやすくなりナビゲーションが容易になります。

</br>
</br>


**ベストプラクティス**

トラフィック管理者、システム管理者、割り当てられたユーザーがイシューに直接取り組むことができるように、リクエストキューレポートを含むダッシュボードを作成して割り当てます。

**その理由は次のとおりです**

ユーザーが受信リクエストにすばやく簡単にアクセスできるようにすると、シャッフルで作業が失われることはありません。

</br>
</br>

**ベストプラクティス**

レイアウトテンプレートを使用して、キューを作成する必要のないユーザー向けに、プロジェクトの左側のパネルメニューからリクエストキューの設定オプションを削除します。


**その理由は次のとおりです**

これにより、すべてのリクエストキューは適切な作成プロセス（ガバナンス委員会によるレビューなど）を経て、システム管理者またはグループ管理者によって正しく設定されます。

さらに、キューリストを整理し、組織で必要なリクエストの種類に焦点を当てることができます。

</br>
</br>

**ベストプラクティス**

ユーザーが Workfront 関連の質問をしたり、システムの設定に関するリクエストを作成したり、新しいユーザーのトレーニングをスケジュールしたりできるように、システム管理者のリクエストキューを作成します。

**その理由は次のとおりです**

これにより、ユーザーが質問を送信したり、管理者が Workfront 関連のイシューを収集、監視、対応したりするための一元化された場所が提供されます。

さらに、この情報を使用して、システム管理者の役割の時間、労力、価値をリーダーシップに示し、システム管理者を追加する正当な理由として使用できます。

</br>
</br>


**ベストプラクティス**

リクエストキューを定期的に監査して、使用されていないキューを識別し、共有しないようにします。

**その理由は次のとおりです**

Adobe Workfront システムの設定と項目を定期的に監査することで、不要な項目をなくし、整理整頓することができます。キューが使用または監視されなくなった場合は、ユーザーをキューにアクセスできないようにして、作業リクエストが無効にならないようにします。

</br>
</br>


**ベストプラクティス**

トピックグループを使用して、リクエストキュー内の 10 個を超えるキューのトピックを整理し、短くて管理しやすいリストを作成します。

**その理由は次のとおりです**

トピックグループを使用すると、選択オプションの初期リストを減らすことで、ユーザーの採用を増加し、混乱を減らすことができます。 これにより、ユーザーはリクエストを送信しようとする際に圧倒されることなく、探しているものを簡単に見つけることができます。

また、システム管理者やリクエストキューマネージャーは、ユーザーにスムーズなナビゲーションパスを作成し、より優れた方法で、送信されるリクエストのタイプを整理してレポートを作成できます。

</br>
</br>

**ベストプラクティス**

複数のキューを作成するのではなく、トピックグループとキューのトピックを使用してリクエストキューを分割することで、ユーザーが使用できるリクエストキューの合計数を制御します。

**その理由は次のとおりです**

リクエストキューが多すぎると、ユーザーが必要なものを見つけるのが困難になります。

また、キューが少ない場合は、トラフィックコーディネーター、システム管理者、またはキューを管理する他のユーザーが、複数のリクエストキューのプロジェクトに移動することなく、必要な情報をより迅速に見つけることができます。

リクエストキューごとに異なるアクセスが必要な場合や、キューの統合によってユーザーが混乱する場合は、複数のリクエストキューを作成します。

</br>
</br>

**ベストプラクティス**

各キューのトピックのルーティングルールを設定します。少なくとも、デフォルトのルーティングルールは設定します。

**その理由は次のとおりです**

ルーティングルールを使用すると、常に受信リクエストが割り当てられ、作業が見落とされることはありません。

</br>
</br>

**ベストプラクティス**

選択的なルーティングが必要な場合は、トピックグループとキューのトピックを活用します。

**その理由は次のとおりです**

ルーティングルールは、カスタムフォームのフィールドには適用できません。 したがって、様々なタイプのリクエストを異なるチームや個人にルーティングする必要がある場合は、リクエストの各タイプに独自のトピックグループやキュートピックを作成し、作業を適切にルーティングできるようにします。

</br>
</br>

**ベストプラクティス**

個人ではなくチームにリクエストをルーティングします。

**その理由は次のとおりです**

リクエストがチームに送信されると、チーム全体が、行われているリクエストと今後の作業の内容を把握できます。全員がチームページで新しい項目を確認したり、ダッシュボードのレポートで最新情報を追跡したりできます。

また、受信リクエストのレビューや割り当てを担当するトラフィック管理者またはその他の担当者が不在の場合、バックアップが自動的に使用可能になり、リクエスト情報にアクセスできるようになります。
