---
title: ISBLANK 式と CONTAINS 式の使用
description: Adobe  [!DNL Workfront] の計算フィールドで ISBLANK 式と CONTAINS 式を使用および作成する方法を説明します。
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: isblank-contains.png
exl-id: 819ffec8-e7e6-4a3c-a589-1348aa09e27d
source-git-commit: 409147f9a62302d28e14b834981992a0421d4e4b
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 64%

---

# ISBLANK 式と CONTAINS 式の使用

CONTAINS 式と ISBLANK 式の両方を使用して、単純な true または false の値を指定します。違いは、ISBLANK 式がフィールドに値を保持しているかどうかをチェックするのに対し、CONTAINS 式はフィールド内の特定の文字列を検索しているという点です。

例えば、プロジェクトに説明が含まれているかどうかを確認するには、ISBLANK 式を使用します。説明フィールドが空白の場合、式は true の値を返します。説明フィールドが空白でない場合は、値 false を返します。

![ワークロードバランサーと稼働率レポート](assets/isblank01.png)

説明内の特定の値（「チャリティイベント」など）を検索するには、「次を含む」というテキスト式を使用します。 説明に「チャリティイベント」が見つかった場合、計算フィールドには「true」と表示されます。 「チャリティーイベント」が見つからない場合は、「false」と表示されます。

![ワークロードバランサーと稼働率レポート](assets/isblank02.png)

## ISBLANK

ISBLANK テキスト式には、式の名前と 1 つのデータポイントが含まれます。

**ISBLANK({data point})**

![ワークロードバランサーと稼働率レポート](assets/isblank03.png)

上の例（プロジェクトに説明が含まれているかどうかを知りる）では、式は次のようになります。

ISBLANK({description})

## 次を含む

「次を含む」のテキスト式には、式の名前、検索する単語または語句、検索するフィールドが含まれます。

**CONTAINS(&quot;phrase&quot;,{fields})**

探している単語やフレーズを必ず引用符で囲んでください。引用符を付けないと、式が無効になります。

上記の例（プロジェクトの説明で「チャリティーイベント」を探す場合）では、式は次のようになります。

**CONTAINS(&quot;チャリティイベント&quot;,{description})**

![ワークロードバランサーと稼働率レポート](assets/isblank04.png)

**メモ**：CONTAINS 式では大文字と小文字が区別されます。例えば、「Charity Event」が説明フィールドで大文字になっている場合、式の中でそのフレーズを大文字にします。

**CONTAINS(&quot;チャリティイベント&quot;,{description})**

ISBLANK 式と CONTAINS 式は、値が存在するかどうかを調べる場合に使用すると便利です。 ただし、値が何であるかを知るには、実際にそれを確認したり、何らかの記述子があった方が、より良い洞察を得ることができるかもしれません。

例えば、プロジェクトがリクエストから転換されたことだけでなく、元のリクエストの名前を知る必要があるとします。

その場合は、CONTAINS 式を IF 式と共に使用します。

ISBLANK テキスト式と CONTAINS テキスト式は、IF テキスト式と一共に使用されることがよくあります。
