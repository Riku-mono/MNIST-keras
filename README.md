# CNNによる手書き文字認識（MNIST）

Google Colab上でCNNによる手書き文字認識（MNIST）を行った。

## 結果

- Train accuracy : 99.97%
- Test accuracy : 99.43%

## モデル

    Input -> [[Conv2D -> relu]*2 -> MaxPool2D -> Dropout]*2 -> Flatten -> Dense -> BatchNormalization -> Dropout -> Dense -> Out

## 注意
データセットを正規化・配列化したものを保存して使用している。
そのため、データセットを各自で用意するか、以下のコードを実行してデータセットを作成する必要がある。