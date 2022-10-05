---
title: 計算フィールドの式について知っておくべきこと
description: でカスタム計算フィールドを使用する際に知っておくとよい概念の一覧を簡単に示します。 [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: to-know-expressions.png
exl-id: 512a3071-f47f-4fd4-bf5f-9b18bef8ba59
source-git-commit: 2b9a31b45ff94222a77c05292ee5b9d8229f5f0b
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 0%

---

# 計算フィールドの式について知っておくべきこと

以下に、 [!DNL Workfront].

## 式名では大文字と小文字は区別されません

式名に関しては、大文字と小文字は関係ありません。 大文字、小文字、またはその両方を使用できます。 式 ISBLANK(Description) を使用すると、「ISBLANK」は次のように記述できます。

* ISBLANK
* Isblank
* IsBlank
* isBLANK

彼らは全てうまくいく。

## 時間は分単位で保存されます

時間 [!DNL Workfront’s] データベースは分単位で保存されます。 「計画時間」や「実際の時間」などのフィールドを参照する場合は、60 で割って時間を分単位で表示し、分単位では表示しません。

## 間隔は式に影響しません

式を記述する場合は、各式の間にスペースをほとんどあるいはまったくない方法を推奨します。

* IF(ISBLANK(Description),&quot;No Description&quot;,&quot;Has Description&quot;)

ただし、間隔が何が起きているかを確認するのに役立つ場合は、式に間隔を追加できます。 余分なスペースを指定しても、式によるでの値の収集や計算が妨げられることはありません。 [!DNL Workfront].

* IF (ISBLANK (Description), &quot;No Description&quot; , &quot;Has Description&quot; )

## 引用符は直線にする必要があります

式に引用符を使用する場合は、引用符がまっすぐ (&quot;) であることを確認してください。 引用符が曲線 (&quot;) の場合、 [!DNL Workfront] 「式が無効です」というメッセージが引き続き表示されます。

## フォームの保存とオブジェクトの編集時に計算を更新

これは、計算フィールドに関して理解しておくべき重要な側面です。

計算フィールドに表示される情報は、カスタムフォームが再計算されない限り、同じままで古くなります。 式は、オブジェクトの [ 詳細 ] メニューの [ 式の再計算 ] オプションを使用して更新できます。

問題が開かれた日数を表示します。 DATEDIFF という式を持つ「Days Open」という計算フィールドを作成します。

* フィールド名=オープン日数
* 式= DATEDIFF（入口日，$$TODAY）

保存後、問題が最初に作成されてからの日数または [!DNL Workfront]また、今日の日付をオブジェクトの詳細ページまたはレポートビューに表示できます。

次の日に同じ詳細ページまたはレポート表示を表示する場合、その数は 1 増分されると予想されます。 今日が 5 の場合は、明日は 6 になるはずです。 次の日は 7、次の日 8、などです。

ただし、フィールドには毎日 5 が表示され続けます。 情報を更新するには、フィールドを「再実行」するか、再計算する必要があります。

「式を再計算」オプションを使用してフィールドを更新するには、次の手順に従います。

* オブジェクトの名前をクリックして開きます。
* その他メニューをクリックします。
* リストから「式の再計算」を選択します。

また、リストまたはレポートで「一括編集」機能を使用して、複数の式を同時に再計算することもできます。 問題のリストを示すレポートを作成し、開いている日数の計算が列に表示されているとします。 すべての問題を一度に再計算する場合は、次の手順に従います。

* レポートですべての問題を選択します。
* 選択したすべての問題を一括編集するには、編集オプションを選択します。
* 左側の Custom Formsラベルをクリックして、カスタムフォームセクションまで下にスクロールします。
* 「カスタムForms」セクションの下部にある「カスタム式を再計算」ボックスをオンにします。
* 「変更を保存」をクリックします。

画面が更新され、計算フィールドに更新された情報が表示されます。

**注意**:計算フィールドの式は更新や再計算の方法は他にもありますが、最も速く簡単な方法です。

## 計算は、同じフィールド内のフォームによって異なる場合があります

計算フィールドをカスタムフォームに保存し、カスタムフォームを保存すると、計算フィールドがフィールドライブラリに追加され、他のカスタムフォームで使用できるようになります。

ただし、フォーム A に計算フィールドがあり、フォーム B に同じ計算フィールドがある場合、最初は計算方法がまったく同じであると考えられます。 必ずしもそうではない。 フォーム A の計算フィールドは、フォーム B の全く異なる方法で計算することができます。

フィールドライブラリから計算済みカスタムフィールドを選択し、カスタムフォームに追加すると、そのフィールドは追加されますが、計算は空白になります。 これが発生する理由の 1 つは、別のオブジェクトタイプに存在しないフィールドを計算が参照している可能性があるためです。

例えば、プロジェクトでタスクを完了するのに要した時間を判断するために、計算フィールド「完了までの日数」を作成したとします。

* WEEKDAYDIFF（実際の開始日，実際の完了日）

繰り返しに対しても同じ処理を実行したい。 同じ式を使用できます。ただし、タスクオブジェクトで使用できるフィールドは、反復オブジェクトでは必ずしも使用できるとは限りません。 そう [!DNL Workfront] を使用すると、正しいオブジェクトフィールドを使用して計算を作成できます。

**ヒント**:カスタムフィールドを作成する際に、計算式を「計算」ボックスから「説明」フィールドにコピーします。 計算済みのカスタムフィールドがフィールドライブラリからカスタムフォームに追加された場合、このフィールドは消去されません。

必要に応じて、カスタムフォームの計算フィールドは非常に単純な場合も、非常に複雑な場合もあります。 式は、他の式や値を埋め込んだり、ネストしたりして、組織でおこなわれている作業の状況をより深く把握するために必要な詳細レベルを提供できます。

<!--Depending on the need, calculated fields in custom forms can be quite simple or very complex. Expressions can embed, or nest, other expressions and values to provide the level of detail needed to get a better picture of what is going on with the work being done at your organization. 

Most of the examples and exercises in this course have been relatively simple to provide a base understanding of the expressions most commonly used and how to build those expressions in a custom calculated field. 

Now you’re ready to start building your own calculated custom fields.-->
