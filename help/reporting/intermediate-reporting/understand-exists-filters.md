---
title: EXISTS フィルターについて
description: EXISTS フィルターの概要、機能、ゼロから作成する方法を説明します。 さらに、EXISTS フィルターの便利な例もたくさん見られます。
activity: use
team: Technical Marketing
feature: Reports and Dashboards
type: Tutorial
role: User
level: Intermediate
jira: KT-1880
last-substantial-update: 2025-08-25T00:00:00Z
doc-type: video
source-git-commit: 7be0b8cce9cba04927d6704d0009b482bbcf4b41
workflow-type: tm+mt
source-wordcount: '682'
ht-degree: 0%

---

# EXISTS フィルターについて

EXISTS フィルターは、標準の Report Builder における 2 つのテーブル/フィールドジャンプの制限を回避できる、高度なテキストモードフィルターです。 または、NOTEXISTS を使用して、特定の関係条件を持たないシステム内のオブジェクトを識別することもできます。

このビデオでは、EXISTS フィルターを作成して、プルーフ承認レポートに「現在のプロジェクトでのプルーフ承認」を表示する方法を説明します。

EXISTS 関数の仕組みに関する詳細な説明については、[EXISTS ステートメントを使用した複雑なテキストモードフィルターの作成 ](https://experienceleague.adobe.com/ja/docs/workfront/using/reporting/reports/text-mode/create-complex-text-mode-filters-using-exists-statements) ドキュメントを参照してください。

>[!VIDEO](https://video.tv.adobe.com/v/3471181/?quality=12&learn=on&enablevpops)

## EXISTS フィルターの例

### プロジェクト報告書は存在します

タスクレベルにある projectID を比較し、それをプロジェクトレベルの ID フィールドと照合することで、タスクをリンクオブジェクトとして使用します。 これにより、タスクの割り当てユーザーを$$USER.ID ワイルドカードと比較できます。 この結果、表示ユーザーがに割り当てられているプロジェクトのみを返すことになります
タスク（プライマリ担当者であるかどうかに関係なく）。

```
EXISTS:A:$$OBJCODE=TASK
EXISTS:A:assignmentsUsersMM:ID=$$USER.ID
EXISTS:A:assignmentsUsersMM:ID_Mod=in
EXISTS:A:projectID=FIELD:ID
```


イシュー（optask）をリンクオブジェクトとして使用し、イシュー（optask）レベルにある projectID を比較して、それをプロジェクトレベルの ID フィールドに一致させます。 次に、これらの問題（optask）のエントリ日が、指定されたスパン内にあるかどうかを確認します。 この場合、を持つプロジェクトが返されます
NOTEXISTS により、過去 30 日間にローリングでログに記録された問題（optask）がありません。

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=OPTASK
EXISTS:A:entryDate=$$TODAY
EXISTS:A:entryDate_Mod=between
EXISTS:A:entryDate_Range=$$TODAY-30d
EXISTS:A:projectID=FIELD:ID
```

### テンプレートレポートが存在する

このフィルターでは、プロジェクトの作成に使用されていない、または過去 1 年間にプロジェクトに添付されたすべてのテンプレートを表示します。 1 つの注意点は、テンプレートが添付ファイルとして使用されたかどうかを判断するには、タスクが含まれているテンプレートに依存することです。

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

### タスク報告書が存在します

User テーブルをリンクオブジェクトとして使用し、割り当て taskID とタスク ID で接続します。 次に、ID のチーム コレクションをユーザーのチーム ID に対してチェックし、担当者のいずれかが表示ユーザーと同じチームに属する場合はタスクを返します。

```
EXISTS:1:$$OBJCODE=USER
EXISTS:1:teams:ID=$$USER.teamIDs
EXISTS:1:userAssignments:taskID=FIELD:ID
```

### ユーザーレポートが存在する

これにより、過去 3 週間に更新を投稿しなかったすべてのユーザーが返されます。 メモオブジェクトを使用してギャップを埋め、ownerID をユーザー ID と比較します。 は、所有するメモのエントリ日が 3 週間前を超えない場合、そのユーザーを返します。

```
EXISTS:A:$$OBJCODE=NOTE
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:ownerID=FIELD:ID
EXISTS:A:entryDate=$$TODAY-3w
EXISTS:A:entryDate_Mod=gt
```

これにより、先週ログ時間を記録していないすべてのユーザーが返されます。 この場合は、上の例に非常に似た方法を使用しますが、代わりに、時間所有者情報および時間のエントリ日を使用して、返されるユーザーのベースを作成します。

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

### カテゴリ （カスタムフォーム） レポートが存在する

このテキストでは、プロジェクトでまったく使用されていないすべてのプロジェクトフォームのリストが示されます。 これは、対象となるフォームのオブジェクトタイプの指定と併せて使用する必要があります。 したがって、この例ではフォーカスは PROJ なので、objTypes 行に引き出し線を含める必要があります。 これは使用できます
他のオブジェクトタイプの場合は、オブジェクトコード関連のパーツを変更します。 これにより、添付されたプロジェクトのコレクションがリストされたフォームにチェックされ、一致するものがない場合は返されます。

```
EXISTS:A:$$OBJCODE=PROJ
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:objectCategories:categoryID=FIELD:ID
objTypes=PROJ
objTypes_Mod=in
```

### パラメーター（カスタムフィールド）レポートが存在する

これは、現在システムのカスタムフォームに添付されていないカスタムフィールドを返します。

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```

### 報告書は存在します

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

### プルーフ承認レポートが存在します

これにより、ステータスが「現在」のプロジェクトに対してのみプルーフの承認が返されます。 これは、Document オブジェクトを使用して、currentVersionID を documentVersionID に確認し、そこからプロジェクトのステータスにジャンプすることで、プルーフの承認からプロジェクトへのギャップを埋めます。

```
EXISTS:1:$$OBJCODE=DOCU
EXISTS:1:currentVersionID=FIELD:documentVersionID
EXISTS:1:project:status=CUR
EXISTS:1:project:status_Mod=in
```
