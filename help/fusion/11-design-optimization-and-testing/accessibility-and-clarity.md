---
title: アクセシビリティと明確さ
description: シナリオを読みやすくし、共有と理解を容易にするための、基本的なベストプラクティスを学びます。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11037
recommendations: noDisplay,catalog
exl-id: ba2c5c64-ab4d-42d3-8a69-6b9df1373b29
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: ht
source-wordcount: '697'
ht-degree: 100%

---

# アクセシビリティと明確さ

Workfront Fusion トレーニングの早い段階で、シナリオを読みやすく、共有と理解を容易にするための基本的なベストプラクティスを学びました。 このプラクティスは、将来の Workfront Fusion ユーザーや、Workfront Fusion インスタンスのトラブルシューティングやサポートを行うすべての人にとって、事案をより簡単にするのに役立ちます。シナリオを設計する際には、以下のガイドラインに従って将来のために役立ててください。

## ラベルとメモ

一般的に Workfront Fusion の主な目的は、常にシンプルなシナリオ設計にしておくことです。 ここでは、解釈しやすいデザインを作成する方法をいくつか紹介します。

* すべてのモジュールに名前が付けられていることを確認します。 モジュールを右クリックし、「名前を変更」を選択します。 モジュールラベルは、モジュールの実行内容に関して、簡潔で理解可能なものにする必要があります。 例えば、「Ch テンプレートを使用した Mktg Proj の作成」などです。
  ![エラー処理を含むシナリオの画像](assets/design-optimization-and-testing-1.png)
* ルーティングパスにもラベルを付けます。 ルーターの直後にフィルターを使用しないパスでも、フィルターロジックを入力せずにラベルを適用できます。これを実行すると、他のユーザーが、どのバンドルがどのパスを渡すのか、およびその理由を理解できます。 フィルターのないルーターパスのラベルを作成するには、パスを右クリックし、ラベルを追加して保存します。
  ![エラー処理を含むシナリオの画像](assets/design-optimization-and-testing-2.png)
* モジュールラベルまたはルーティングパスラベルが短すぎて実際に何が起こっているのかを明確にできない場合には、シナリオの該当する個所にメモを追加します。設計および反復処理のプロセス全体を通して、いつでもメモを追加できます。

ただし、開始の準備が整ったときにシナリオデザインの一番後ろにメモが追加されていると、最も読みやすく理解しやすいでしょう。シナリオデザインの最後（最下部、右隅）からさかのぼって作業します。こうすることで、シナリオの最初に適用されるメモが、メモパネルを開いたときに、リストの一番上に表示されます。

メモパネルを保存または閉じた後、メモは、最も新しく作成されたものが一番上に並べ替えられます。 下の画像では、最初に作成したメモがリストの一番下に表示されています。 メモは意図的に右下から上のパス、そして最後にトリガーまで作成されています。これは基本的に、データの束がシナリオを通過する順序とは逆です。これにより、データの束でシナリオが実際に実行される順序でメモが表示されます。

![エラー処理を含むシナリオの画像](assets/design-optimization-and-testing-3.png)

## Workfront Fusion テンプレート

テンプレートの使用は、モジュールやルーティングパスのラベル付けを効率化する優れた方法です。 ベストプラクティステンプレートを使用すると、一般的なユースケースのシナリオを素早く作成できます。

### テンプレートの例

シナリオを開始する際は、まず、役立つテンプレートが使用可能かどうかを確認します。 例えば、Workfront から CSV ドキュメントをダウンロードして解析するシナリオを作成するとします。

「テンプレート」セクションをクリックして、必要を満たす公開テンプレートがあるかどうかを確認します。

![エラー処理を含むシナリオの画像](assets/design-optimization-and-testing-4.png)

「チームテンプレート」タブをクリックして、チームの誰かが役に立ちそうなテンプレートを作成したかどうかを確認します。

使用したいテンプレートが見つかった場合は、テンプレート名をクリックして開きます。

![エラー処理を含むシナリオの画像](assets/design-optimization-and-testing-5.png)

次に右上隅に移動し、オプションをクリックし、「シナリオを作成」を選択します。

![エラー処理を含むシナリオの画像](assets/design-optimization-and-testing-6.png)

### テンプレートの作成

テンプレートは、「チームテンプレート」セクションで作成できます。 作成したテンプレートは、作成者とチームが使用できますが、「公開」ボタンをクリックすると、チーム外のユーザーと共有できます。

![エラー処理を含むシナリオの画像](assets/design-optimization-and-testing-7.png)

テンプレートを作成するときは、ウィザードを含めることができます。ウィザードは、ユーザーがシナリオを作成し、接続、マップされたデータ、およびその他のパネルフィールドを適切に変更できるように、テンプレートを使用するユーザーをガイドするものです。

テンプレートを使用してシナリオを作成する際に使用できる説明手順を追加するには、「ウィザードで使用」チェックボックスをオンにします。この情報は、ヘルプフィールドに表示されます。 テンプレートの使用時にユーザーがこのテキストを表示するには、「デフォルト値として使用」を有効にします。

![エラー処理を含むシナリオの画像](assets/design-optimization-and-testing-8.png)

## 詳細情報 以下をお勧めします。

[Workfront Fusion ドキュメント](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=ja)
