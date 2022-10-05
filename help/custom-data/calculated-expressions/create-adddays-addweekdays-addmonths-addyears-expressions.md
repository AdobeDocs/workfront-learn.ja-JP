---
title: ADDDAYS、ADDWEEKDAY、ADDMONTHS、ADDYEARS 式の作成
description: Adobeの計算フィールドで ADD 式を使用および作成する方法を説明します [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335175.png
kt: 8912
exl-id: f194fbc8-99b3-4fed-9fc5-a2f5fa4593d2
source-git-commit: 2b9a31b45ff94222a77c05292ee5b9d8229f5f0b
workflow-type: tm+mt
source-wordcount: '271'
ht-degree: 0%

---

# ADDDAYS、ADDWEEKDAY、ADDMONTHS、ADDYEARS 式の作成

このビデオでは、次のことを学習します。

* ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR 式で計算される値
* 計算フィールドで ADDWEEKDAYS データ式を作成する方法

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12)

## その他の例

ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR 式の追加Adobeを以下に示します [!DNL Workfront] のお客様が作成されました。

**は次の方法で実行する必要があります：**

顧客は、実際の開始日と計画期間に基づいて、タスクがいつ完了したかを知りたがりました。 この場合、タスクが遅れている場合に移動する可能性があるので、「予定完了日」は機能しません。また、前のタスクで遅延が生じた場合は、「計画完了日」は役に立ちません。

作成された式は ADDDAYS( 実際の開始日，（期間/480）) です

「期間」フィールドの時間は分単位で保存されます。 したがって、この式では、時間を日数で反映する場合、「期間」フィールドを単独で使用することはできません。 そのためには、期間を 480 分で割る必要があります（480 分= 8 時間= 1 日）

2 番目の値スロットには (Duration/480) が含まれるのはこのためです。


**請求書の完了日**

この例では、既にシステムで作成および保存されている別の計算フィールドを式内に含めます。

顧客は、カスタムフォームのカスタム日付フィールド（「請求書送信日」）を使用して請求書が送信された日付を取得していました。 送信後 30 日が経過し、請求書が完成し、提出されます。 この完了日と申告日を自動的に生成するために、ADDDAYS と「請求書発行日」フィールドを使用して計算フィールドを作成しました。 式は次のようになります。

ADDDAYS（請求書発行日，30）
