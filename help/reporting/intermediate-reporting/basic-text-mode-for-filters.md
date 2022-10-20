---
title: フィルターの基本的なテキストモードについて
description: テキストモードとは何か、キャメルケースとは何か、およびのレポートフィルターで使用できる基本的な「プラグアンドプレイ」テキストモードについて説明します。 [!DNL  Workfront].
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
source-git-commit: 7a4649644a99eafd521895133a321f8ea0ff6041
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# フィルターの基本的なテキストモードについて

このビデオでは、次のことを学習します。

* テキストモード
* ラクダの例とは
* レポートフィルターで使用できる基本的な「プラグアンドプレイ」テキストモード

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12)

次のテキストモードでは、ユーザーが「Done with My Part」とマークしたタスクが除外されます。 必要な操作は、タスクフィルターを作成し、必要なフィルタールールを追加してから、テキストモードに切り替えて、フィルターに表示される任意のテキストモードの後に下のコードを貼り付けるだけです。

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

## アクティビティ：テキストモードに関する質問

1. 「ID で入力済み」というタイトルのフィールドのキャメルケースを作成する方法を教えてください。
1. 問題レポートで、フィルターを作成して、クローズ済みとマークされているが承認待ちの問題を表示します。

## 回答

1. 「ID 別に入力」フィールドのキャメルケースは、enteredByID のように記述する必要があります。
1. 問題レポートフィルターのテキストモードは次のようになります。

   ![テキストモードで新しいフィルターを作成するための画面の画像](assets/btm-answer.png)
