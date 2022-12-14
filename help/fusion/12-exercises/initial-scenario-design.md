---
title: 初期シナリオのデザイン
description: 最初のシナリオの構築と共に、Workfront Fusion に初めてログインする際の基本的なナビゲーションヒントをいくつか説明します。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11038
thumbnail: KT11038.png
exl-id: 8ecf4979-f291-4788-bdaa-ab5485fb0849
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 0%

---

# 初期シナリオのデザイン

最初のシナリオの構築と共に、Workfront Fusion に初めてログインする際の基本的なナビゲーションヒントをいくつか説明します。

## 演習の概要

Workfrontで、プロジェクトリスト CSV ファイルの各行に対して新しいプロジェクトを作成します。

![初期シナリオデザイン画像 1](../12-exercises/assets/initial-scenario-design-1.png)

## 従う手順

1. 「Fusion enablement exercises」という名前のフォルダを「Scenario」セクションに作成します。
1. フォルダー内をクリックし、「新しいシナリオを作成」をクリックします。

   ![初期シナリオデザイン画像 2](../12-exercises/assets/initial-scenario-design-2.png)

1. 次のページで、「 Workfront 」を検索してそのアプリを選択します。 次に、「続行」をクリックします。
1. シナリオデザイナー画面の左上で、シナリオの名前を「初期のシナリオデザイン」に変更します。
1. 画面の中央にある空のトリガーモジュールをクリックし、Workfrontアプリを選択して、ドキュメントをダウンロードモジュールを選択します。

   **モジュールのWorkfrontアカウントへの接続を認証します。**

1. 接続を初めて作成する場合は、「追加」ボタンをクリックします。

   ![初期シナリオデザイン画像 3](../12-exercises/assets/initial-scenario-design-3.png)

1. 接続に名前を付けます (「My Workfront 2020」など )。

   ![初期シナリオデザイン画像 4](../12-exercises/assets/initial-scenario-design-4.png)

1. Workfrontインスタンスの URL を入力し、「次へ」をクリックします。

   ![初期シナリオデザイン画像 5](../12-exercises/assets/initial-scenario-design-5.png)

1. パスワードを入力し、「ログイン」をクリックします。

   **接続が確立されました。 次に、Workfrontからダウンロードするドキュメントのドキュメント ID を入力します。**

   ![初期シナリオデザイン画像 7](../12-exercises/assets/initial-scenario-design-7.png)

1. Workfrontに戻ります。 「Fusion Exercise Files」フォルダで、「_Fusion2020_Project List.csv」を選択し、左パネルの「ドキュメントの詳細」をクリックします。 URL アドレスからドキュメント ID 番号をコピーします（URL の最初の長い番号です）。

   ![初期シナリオデザイン画像 8](../12-exercises/assets/initial-scenario-design-8.png)

1. Fusion に戻り、「ドキュメント ID」フィールドに番号を貼り付け、「OK」をクリックします。
1. ベストプラクティスは、モジュールの作成時に名前を変更することです。 Workfrontモジュールを右クリックし、「名前を変更」を選択します。 モジュールに「Get project list」という名前を付けます。

   **次に、ダウンロードした CSV ファイルを解析し、ファイルの各行にアクセスできるようにします。 この情報は、各行からプロジェクトを作成する際に使用します。**

1. 別のモジュールを追加するには、Workfrontモジュールの右側をクリックします。 CSV アプリを検索し、「 CSV を解析」モジュールを選択します。
1. 6 列に対して CSV を解析を設定し、CSV にヘッダー、Comma delimiterType、および CSV フィールドにデータを入力します。 「OK」をクリックします。

   ![初期シナリオデザイン画像 9](../12-exercises/assets/initial-scenario-design-9.png)

1. このモジュールの名前を「Parse project list」に変更します。
1. シナリオデザイナの下部で、「保存」をクリックして、シナリオを保存します。
1. 「1 回実行」をクリックして出力を表示します。

   >[!NOTE]
   >
   >変換サービスを最後のモジュールにすべきでないという警告を無視します（これは true ですが、このテストでは問題になりません）。 [ 実行 ] をクリックします。

   ![初期シナリオデザイン画像 10](../12-exercises/assets/initial-scenario-design-10.png)

1. 「 CSV を解析」モジュールで実行インスペクターを開き、モジュールの入力と出力を確認します。 入力として 1 つのバンドル（CSV ファイル）、出力として複数のバンドル（CSV ファイルの各行に 1 つのバンドル）があります。 次のようになります。

   ![初期シナリオデザイン画像 11](../12-exercises/assets/initial-scenario-design-11.png)

   **モジュールを追加して、CSV ファイルの各行のプロジェクトを作成します。**

1. 別のモジュールを追加します。 Workfrontアプリを選択し、レコードを作成モジュールを選択します。
1. 「レコードタイプ」を「プロジェクト」に設定します。

   >[!TIP]
   >
   >次のような文字を入力して検索します。 *proj*、右に移動します。

1. 次に、Cmd/Ctrl+G キーを使用して名前（プロジェクト名）を検索します。 「名前」の横のチェックボックスをオンにします。フィールドは下に表示されます。
1. 「計画開始日」と「優先度」の横にあるチェックボックスをオンにします。
1. 「名前」フィールドをクリックすると、マッピングパネルが表示されます。 「 CSV を解析」モジュールの「列 1 」フィールドをクリックして、「名前」フィールドに追加します。 CSV ファイルのプロジェクト名です。
1. 「計画開始日」で、「 CSV を解析」モジュールの「列 5 」をクリックします。
1. [ 優先度 ] で、ドロップダウンメニューから [ 標準 ] を選択します。

   **マッピングパネルは次のようになります。**

   ![初期シナリオデザイン画像 12](../12-exercises/assets/initial-scenario-design-12.png)

1. 「OK」をクリックします。

   >[!NOTE]
   >
   >「OK」をクリックせずに誤ってデザイナーに戻った場合、作業内容は保存されず、再度マッピングする必要があります。

1. Workfrontモジュールを右クリックし、名前を「Workfrontプロジェクトの作成」に変更します。
1. シナリオを保存し、「 1 回実行」ボタンをクリックします。
1. 最後のモジュールの右上にある実行インスペクターをクリックします。

   + 20 個の操作が実行されました。 各操作では、CSV ファイルから 1 行のバンドル（1 行）を入力および出力 1 つのバンドル (Workfrontで作成されたプロジェクト ) として取得しました。 作成したプロジェクトのプロジェクト ID が出力バンドルと共に表示されます。

   ![初期シナリオデザイン画像 13](../12-exercises/assets/initial-scenario-design-13.png)

   **メモの使用**

1. メモは、シナリオのデザインをより明確に把握するのに役立ちます。 「 Workfrontプロジェクトを作成」モジュールにメモを追加するには、右クリックして「メモを追加」を選択します。 デザイナーウィンドウの右側にあるパネルがポップアウト表示され、モジュールにメモを追加できます。 「CSV ファイルからマッピングされた名前、計画開始日、優先度を使用してプロジェクトを作成します。」と入力します。
1. トリガーモジュール ( 最初のWorkfrontモジュール ) が何をしているかを説明するメモを追加します。
1. ノートパネルを閉じるには、右上隅の X をクリックします。

   + メモに再度アクセスするには、下部のツールバーのメモボタンをクリックするか、モジュールを右クリックして新しいメモを追加します。
   + メモは時系列順に逆順に並べ替えられます。
   + メモを追加すると、[ メモ ] ボタンにオレンジ色の点が表示されます。

   ![初期シナリオデザイン画像 14](../12-exercises/assets/initial-scenario-design-14.png)

1. コントロールツールバーの「保存」ボタンをクリックして、シナリオを保存します。
1. Workfrontインスタンスで作成されたプロジェクトを表示できます。
