---
title: ADDDAYS、ADDWEEKDAY、ADDMONTHS、ADDYEARS 式の作成
description: Adobe  [!DNL Workfront] の計算フィールドで ADD 式を使用および作成する方法を説明します。
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335175.png
jira: KT-8912
exl-id: f194fbc8-99b3-4fed-9fc5-a2f5fa4593d2
doc-type: video
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: ht
source-wordcount: '281'
ht-degree: 100%

---

# ADDDAYS、ADDWEEKDAY、ADDMONTHS、ADDYEARS 式の作成

このビデオでは、次のことを学習します。

* ADDDAYS 式、ADDWEEKDAY 式、ADDMONTHS 式、ADDYEAR 式で計算すること
* 計算フィールドで ADDWEEKDAYS データ式を作成する方法

>[!VIDEO](https://video.tv.adobe.com/v/3416191/?quality=12&learn=on&enablevpops&captions=jpn)

## その他の例

Adobe Workfront のお客様が作成した、その他の ADDDAYS 式、ADDWEEKDAY 式、ADDMONTHS 式、ADDYEAR 式を以下に示します。

**完了期限**

そのお客様は、実際の開始日と予定期間に基づいて、タスクをいつ完了する必要があったかを知りたいと考えました。この場合、予定完了日は機能しません。予定完了日は、タスクが遅れていると移動する可能性があり、前のタスクに遅延がある場合は役に立たないためです。

作成された式は ADDDAYS({actualStartDate},{durationMinutes}/480) でした。

「期間」フィールドの時間は分単位で保存されます。したがって、この式では、時間を日数で反映する場合、「期間」フィールドを単独で使用することはできません。そのためには、期間を 480 分で割る必要があります（1 日 = 8 時間 = 480 分）。

2 番目の値スロットに (Duration/480) が含まれるのはこのためです。


**請求書の完了日**

この例には、ADDDAYS 式を使用するだけでなく、以前にカスタムフォームで作成および保存したカスタムフィールドも含まれます。

顧客は「請求書の送信日」というタイトルのカスタム日付フィールドを使用して、請求書が送信された日付を取得します。

送信後、請求書は 30 日以内に完了し、提出する必要があります。この完了日と提出日を自動的に生成するには、ADDDAYS 計算フィールドと「請求書の提出日」カスタムフィールドを使用します。式は次のようになります。

ADDDAYS({DE:Invoice Submission Date},30)
