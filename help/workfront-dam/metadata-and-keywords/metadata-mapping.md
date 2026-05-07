---
title: メタデータマッピングの設定
description: '[!UICONTROL Workfront DAM] のメタデータマッピングを設定する方法について説明します。'
activity: use
team: Technical Marketing
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
jira: KT-10088
exl-id: 3869db93-9fbc-4689-b838-0f4400a436c3
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T22:32:59.006Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 276
ht-degree: 100%

---

# メタデータマッピングの設定

アセットに関する [!DNL Workfront] 関連の情報は、アセットと共に [!DNL Workfront] から [!UICONTROL Workfront DAM] に転送できます。 [!DNL Workfront] [!UICONTROL 設定]エリアのメタデータマッピングオプションにより、この情報の転送が可能になります。

メタデータマッピングの設定に関するベストプラクティスのレコメンデーションについては、[!DNL Workfront] コンサルタントにお問い合わせください。

メタデータマッピングを設定するには、[!DNL Workfront] 管理者および [!UICONTROL Workfront DAM] 管理者である必要があります。 開始する前に、[!DNL Workfront] と [!UICONTROL Workfront DAM] アカウントを接続する必要があります。

## アカウントの接続

1. [!DNL Workfront] にログインします。
1. プロジェクト、タスクまたはイシューを開き、「**[!UICONTROL ドキュメント]**」タブをクリックします。
1. 「**[!UICONTROL 新規追加]**」ボタンをクリックし、ドロップダウンメニューから「**[!UICONTROL Workfront DAM から]**」を選択します。
1. 表示される [!UICONTROL Workfront DAM] 認証ボックスにログイン名とパスワードを入力します。
1. 次に、「**[!UICONTROL はい]**」をクリックして、[!UICONTROL DAM] アカウントに [!DNL Workfront] のアクセス権を付与します。
1. 必要に応じて、ページを更新し、[!UICONTROL Workfront DAM] へのアクセス権を更新します。

この接続が確立されると、2 つのシステム間でメタデータのマッピングを開始できるようになります。 マッピングを開始する前に、必要なメタデータフィールドが [!UICONTROL Workfront DAM] に既に作成されていることを確認します。

## マッピングの設定

1. [!DNL Workfront] にログインします。
1. [!UICONTROL メインメニュー]から「**[!UICONTROL 設定]**」を選択します。
1. 左側のパネルメニューで「**[!UICONTROL ドキュメント]**」セクションを展開します。
1. 次に、「**[!UICONTROL メタデータマッピング]**」をクリックします。
1. Workfront フィールドに、マッピングする [!DNL Workfront] フィールドのフィールドソースを入力します。
1. 次に、対応するまたはターゲットの **[!UICONTROL Workfront DAM]** メタデータフィールドを選択します。
1. 「**[!UICONTROL マッピングを追加]**」ボタンをクリックします。
1. ウィンドウの下部にあるグラフに、[!UICONTROL Workfront フィールドソース]と [!UICONTROL Workfront DAM ターゲットフィールド]が表示されます。
1. 必要なすべてのメタデータフィールドに対して繰り返します。

![ の[!UICONTROL メタデータマッピング]画面のスクリーンショット[!DNL Workfront]](assets/01-metadata-mapping.png)
