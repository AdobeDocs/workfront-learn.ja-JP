---
title: '[!UICONTROL Workfront DAM] のメタデータマッピングの設定'
description: '[!UICONTROL Workfront DAM] のメタデータマッピングを設定する方法について説明します。'
activity: use
team: Technical Marketing
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
jira: KT-10088
exl-id: 3869db93-9fbc-4689-b838-0f4400a436c3
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 100%

---

# メタデータマッピング

アセットに関する [!DNL Workfront] 関連の情報は、アセットと共に [!DNL Workfront] から [!UICONTROL Workfront DAM] に転送できます。[!DNL Workfront] [!UICONTROL 設定]エリアのメタデータマッピングオプションにより、この情報の転送が可能になります。

メタデータマッピングの設定に関するベストプラクティスの推奨事項については、[!DNL Workfront] コンサルタントにお問い合わせください。

メタデータマッピングを設定するには、[!DNL Workfront] 管理者および [!UICONTROL Workfront DAM] 管理者である必要があります。開始する前に、[!DNL Workfront] と [!UICONTROL Workfront DAM] アカウントを接続する必要があります。

## アカウントの接続

1. [!DNL Workfront] にログインします。
1. プロジェクト、タスクまたはイシューを開き、「**[!UICONTROL ドキュメント]**」タブをクリックします。
1. 「**[!UICONTROL 新規追加]**」ボタンをクリックし、ドロップダウンメニューから「**[!UICONTROL Workfront DAM から]**」を選択します。
1. 表示される [!UICONTROL Workfront DAM] 認証ボックスにログイン名とパスワードを入力します。
1. 次に、「**[!UICONTROL はい]**」をクリックして、[!UICONTROL DAM] アカウントに [!DNL Workfront] のアクセス権を付与します。
1. 必要に応じて、ページを更新し、[!UICONTROL Workfront DAM] へのアクセス権を更新します。

この接続が確立されると、2 つのシステム間でメタデータのマッピングを開始できるようになります。マッピングを開始する前に、必要なメタデータフィールドが [!UICONTROL Workfront DAM] に既に作成されていることを確認します。

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
