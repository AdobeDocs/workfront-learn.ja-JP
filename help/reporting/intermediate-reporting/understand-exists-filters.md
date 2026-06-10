---
title: 複雑なレポート用のEXISTS フィルターの作成
description: EXISTS フィルターの概要、機能、ゼロから作成する方法を学習します。 さらに、EXISTS フィルターの便利な例も多数紹介します。
activity: use
team: Technical Marketing
feature: Reports and Dashboards
type: Tutorial
role: User
level: Intermediate
jira: KT-18808
last-substantial-update: '2025-08-25T00:00:00.000Z'
doc-type: video
exl-id: f518a919-0c44-4122-873a-e2f10e3162d5
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: c6dd2ac5-f5bd-4e59-9101-25b156918623
subfeature_v2: id: cec4c78b-dd2b-46ec-b824-6ca30f0eb7b2
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-06T02:08:32.688Z'
source-git-commit: 082aa48e99d6c772c973f9bbbc90b0544103e0d5
workflow-type: tm+mt
source-wordcount: 706
ht-degree: 89%

---

# 複雑なレポート用のEXISTS フィルターの作成

EXISTS フィルターは、標準の Report Builder における 2 つのテーブルやフィールドジャンプの制限を回避できる、高度なテキストモードフィルターです。 または、NOTEXISTS を使用して、特定の関係条件を持たないシステム内のオブジェクトを識別することもできます。

このビデオでは、EXISTS フィルターを作成して、プルーフ承認レポートに「現在のプロジェクトでのプルーフ承認」を表示する方法を説明します。

EXISTS の機能に関する詳細な説明については、[EXISTS ステートメントを使用した複雑なテキストモードフィルターの作成](https://experienceleague.adobe.com/ja/docs/workfront/using/reporting/reports/text-mode/create-complex-text-mode-filters-using-exists-statements)ドキュメントを参照してください。

>[!VIDEO](https://video.tv.adobe.com/v/3471181/?quality=12&learn=on&enablevpops=1)

## EXISTS フィルターの例

### プロジェクトレポート EXISTS

タスクレベルにある projectID を比較し、それをプロジェクトレベルの ID フィールドと一致させることで、タスクをリンクオブジェクトとして使用します。 これにより、タスクに割り当てられたユーザーを $$USER.ID ワイルドカードと比較できます。 この結果、表示ユーザーがに割り当てられているプロジェクトのみを返します。
プライマリ担当者かどうかに関係なく、タスクを割り当てます。

```
EXISTS:A:$$OBJCODE=TASK
EXISTS:A:assignmentsUsersMM:ID=$$USER.ID
EXISTS:A:assignmentsUsersMM:ID_Mod=in
EXISTS:A:projectID=FIELD:ID
```


イシュー（optask）をリンクオブジェクトとして使用し、イシュー（optask）レベルにある projectID を比較して、それをプロジェクトレベルの ID フィールドに一致させます。 次に、これらのイシュー（optask）の入力日が指定されたスパン内にあるかどうかを確認します。 この場合、このフィールドの値が
notexistsが原因で、過去30日間にローリングで問題（optask）がログに記録されませんでした。

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=OPTASK
EXISTS:A:entryDate=$$TODAY
EXISTS:A:entryDate_Mod=between
EXISTS:A:entryDate_Range=$$TODAY-30d
EXISTS:A:projectID=FIELD:ID
```

### テンプレートレポート EXISTS

このフィルターでは、プロジェクトの作成に使用されていない、または過去 1 年間にプロジェクトに添付されたすべてのテンプレートを表示します。 注意すべき点は、テンプレートが添付ファイルとして使用されたかどうかを判断するには、タスクが含まれているテンプレートによるということです。

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=TASK
EXISTS:A:entryDate=$$TODAY-1y
EXISTS:A:entryDate_Mod=gte
EXISTS:A:templateTask:templateID=FIELD:ID
EXISTS:B:$$EXISTSMOD=NOTEXISTS
EXISTS:B:$$OBJCODE=PROJ
EXISTS:B:entryDate=$$TODAY-1y
EXISTS:B:entryDate_Mod=gte
EXISTS:B:templateID=FIELD:ID
```

### タスクレポート EXISTS

ユーザーテーブルをリンクオブジェクトとして使用し、割り当て taskID とタスク ID で接続します。 次に、ID のチームコレクションをユーザーのチーム ID に対してチェックし、担当者のいずれかが表示ユーザーと同じチームに属する場合はタスクを返します。

```
EXISTS:1:$$OBJCODE=USER
EXISTS:1:teams:ID=$$USER.teamIDs
EXISTS:1:userAssignments:taskID=FIELD:ID
```

### ユーザーレポート EXISTS

これにより、過去 3 週間に更新を投稿していないすべてのユーザーが返されます。 メモオブジェクトを使用してギャップを埋め、ownerID をユーザー ID と比較します。 所有するメモに、入力日が 3 週間より前のものがない場合、そのユーザーを返します。

```
EXISTS:A:$$OBJCODE=NOTE
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:ownerID=FIELD:ID
EXISTS:A:entryDate=$$TODAY-3w
EXISTS:A:entryDate_Mod=gt
```

これにより、過去 1 週間に時間を記録していないすべてのユーザーが返されます。 上の例に非常に似た方法を使用しますが、代わりに、時間所有者情報および時間の入力日を使用して、返されるユーザーを決定します。

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=HOUR
EXISTS:A:entryDate=$$TODAY-1w
EXISTS:A:entryDate_Mod=gte
EXISTS:A:ownerID=FIELD:ID
```

ユーザーレポートで、プロジェクトの「ユーザー」タブに一致するユーザーのリストを表示します。

```
EXISTS:1:$$OBJCODE=PRTU
EXISTS:1:projectID=<projectID>
EXISTS:1:userID=FIELD:ID
```

### カテゴリ（カスタムフォーム）レポート EXISTS

このテキストには、プロジェクトでまったく使用されたことがないすべてのプロジェクトフォームのリストが示されます。 これは、対象となるフォームのオブジェクトタイプの指定と併せて使用する必要があります。 したがって、この例では焦点は PROJ なので、objTypes 行にコールアウトを含める必要があります。 これは使用可能です
オブジェクトコード関連部分を変更することで、その他のオブジェクトタイプ用に設定できます。 これにより、添付されたプロジェクトのコレクションがリストされたフォームに対してチェックされ、一致するものがなければ結果を返します。

```
EXISTS:A:$$OBJCODE=PROJ
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:objectCategories:categoryID=FIELD:ID
objTypes=PROJ
objTypes_Mod=in
```

### パラメーター（カスタムフィールド）レポート EXISTS

これは、現在、システムのカスタムフォームに添付されていないカスタムフィールドを返します。

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```

### レポートレポート EXISTS

これにより、フィルターで特定の値を使用しているレポートが返されます。

```
EXISTS:1:$$OBJCODE=UIFT
EXISTS:1:ID=FIELD:filterID
EXISTS:1:preference:value=<value here>
EXISTS:1:preference:value_Mod=cicontains
```

これにより、任意のダッシュボードに添付されたレポートが返されます。

```
EXISTS:A:$$OBJCODE=PRTBSC
EXISTS:A:internalSectionID=FIELD:ID
EXISTS:A:portalTab:ID_Mod=notblank
```

### プルーフ承認レポート EXISTS

これにより、ステータスが「現在」のプロジェクトに対してのみプルーフの承認が返されます。 これは、ドキュメントオブジェクトを使用して、currentVersionID を documentVersionID に対して確認し、そこからプロジェクトのステータスにジャンプすることで、プルーフの承認からプロジェクトまでのギャップを埋めます。

```
EXISTS:1:$$OBJCODE=DOCU
EXISTS:1:currentVersionID=FIELD:documentVersionID
EXISTS:1:project:status=CUR
EXISTS:1:project:status_Mod=in
```
