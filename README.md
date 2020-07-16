# 胸部X線画像に対するDCGANの適用

## 参考

- [胸部X線画像を対象とした敵対的生成ネットワーク - DCGAN -](https://qiita.com/tatsunidas/items/779ebe6e403b9b3e85f7)
- [画像の前処理](https://keras.io/ja/preprocessing/image/)
- [Keras - Keras の ImageDataGenerator を使って学習画像を増やす](https://www.pynote.info/entry/keras-image-data-generator#%E5%90%84%E7%94%BB%E7%B4%A0%E5%80%A4%E3%81%AB%E5%80%A4%E3%82%92%E8%B6%B3%E3%81%99)

## トレーニング画像
- [MINIJSRT_DATABASE](http://imgcom.jsrt.or.jp/minijsrtdb/)

## トレーニング画像の処理
1. 上記サイトの「SuperResolution」の256x256, Gray: 8bitをダウンロード
2. ダウンロードしたデータの`org/`内の画像を取り出す
3. `/dataset/train/`フォルダを作ってその中に2で取り出した画像を入れる

## 入力と出力
- 入力：32x32x1の画像247枚
- 出力：32x32x1の画像

## 訓練過程
[![Image from Gyazo](https://i.gyazo.com/6080fa06af6a1cff0ace317e42451fe9.png)](https://gyazo.com/6080fa06af6a1cff0ace317e42451fe9)
