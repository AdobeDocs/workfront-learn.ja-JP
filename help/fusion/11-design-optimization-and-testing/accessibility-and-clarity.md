---
title: アクセシビリティと明快さ
description: シナリオを読みやすく、共有し、理解しやすくするための基本的なベストプラクティスをいくつか学びます。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11037
exl-id: ba2c5c64-ab4d-42d3-8a69-6b9df1373b29
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 0%

---

# アクセシビリティと明快さ

Workfront Fusion トレーニングの初めに、シナリオを読みやすく、共有し、理解しやすくするための基本的なベストプラクティスを学びました。 これらのプラクティスは、今後のWorkfront Fusion ユーザーや、Workfront Fusion インスタンスのトラブルシューティングやサポートをおこなうすべてのユーザーにとって、より簡単な作業をおこなうのに役立ちます。 シナリオを設計する際は、次のガイドラインに従って前払いを行ってください。

## ラベルとメモ

一般的に、Workfront Fusion の主な目的は、常にシンプルなシナリオ設計を持つことです。 簡単に解釈できるデザインを作成する方法を次に示します。

* すべてのモジュールに名前を付けていることを確認します。 モジュールを右クリックし、「名前を変更」を選択します。 モジュールラベルは、モジュールの実行内容に関しては、短いが理解可能である必要があります。 例えば、「Ch テンプレートを使用した Mktg Proj の作成」などです。
   ![エラー処理を含むシナリオの画像](assets/design-optimization-and-testing-1.png)
* ルーティングパスにもラベルを付けます。 ルータの直後にフィルタを使用しないパスでも、フィルタロジックを入力せずにラベルを適用できます。 これを実行すると、他のユーザーは、バンドルがどのパスと理由を渡すかを理解できます。 フィルタのないルータパスのラベルを作成するには、パスを右クリックし、ラベルを追加して、保存します。
   ![エラー処理を含むシナリオの画像](assets/design-optimization-and-testing-2.png)
* モジュールのラベルまたはルーティングパスのラベルが短すぎて実際に何が起きているかを明確にする場合は、シナリオで該当する場合はメモを追加します。 設計および反復処理のプロセス全体を通して、必要に応じてメモを追加できます。

ただし、を起動する準備ができたら、シナリオデザインの最後にメモを追加すると、読んで理解しやすくなる場合があります。 シナリオのデザインの最後（右端と右端）から後方に向かって作業します。 これにより、シナリオの最初に適用されるメモは、メモパネルを開く際にリストの一番上に表示されます。

メモパネルを保存または閉じた後、メモは、最も新しく作成されたメモが一番上に並べ替えられます。 下の画像では、最初に作成したメモがリストの下部に表示されます。 メモは、下から右上のパス、最後にトリガーに対して意図的に作成されています。つまり、データのバンドルがシナリオを通過する順序は逆です。 これにより、データのバンドルでシナリオが実際に実行される順序でメモが表示されます。

![エラー処理を含むシナリオの画像](assets/design-optimization-and-testing-3.png)

## Workfront Fusion テンプレート

モジュールやルーティングパスのラベル付けを効率化する優れた方法は、テンプレートを使用することです。 ベストプラクティステンプレートを使用すると、一般的な使用例で使用するシナリオの作成を迅速におこなうことができます。

### テンプレートの例

シナリオを開始する際は、まず、役立つテンプレートが使用可能かどうかを確認します。 例えば、Workfrontから CSV ドキュメントをダウンロードしてから解析するシナリオを作成するとします。

「テンプレート」セクションをクリックして、必要に応じた公開テンプレートがあるかどうかを確認します。

![エラー処理を含むシナリオの画像](assets/design-optimization-and-testing-4.png)

[ チームテンプレート ] タブをクリックして、チームの誰かが役に立つテンプレートを作成したかどうかを確認します。

使用するテンプレートが見つかった場合は、名前をクリックして開きます。

![エラー処理を含むシナリオの画像](assets/design-optimization-and-testing-5.png)

次に、右上隅に移動し、「オプション」をクリックし、「シナリオを作成」を選択します。

![エラー処理を含むシナリオの画像](assets/design-optimization-and-testing-6.png)

### テンプレートの作成

テンプレートは、「チームテンプレート」セクションで作成できます。 作成したテンプレートは、自分とチームが使用できますが、「公開」ボタンをクリックすると、チーム外のユーザーと共有できます。

![エラー処理を含むシナリオの画像](assets/design-optimization-and-testing-7.png)

テンプレートを作成する際に、ウィザードを含めて、テンプレートを使用するユーザーがシナリオを構築し、接続、マッピングされたデータ、およびその他のパネルフィールドを必要に応じて変更できます。

テンプレートを使用してシナリオを作成する際に使用できる手順を追加するには、「ウィザードで使用」チェックボックスをオンにします。 この情報は、「ヘルプ」フィールドに表示されます。 テンプレートの使用時にユーザーにこのテキストを表示させるには、「デフォルト値として使用」を有効にします。

![エラー処理を含むシナリオの画像](assets/design-optimization-and-testing-8.png)

## 詳細情報 以下をお勧めします。

[Workfront Fusion ドキュメント](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
