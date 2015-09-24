# 起動方法 #

新しく作ったWindows Mugen Plusのフォルダに上書きして
ikemen.exeを起動してください。

# config.ssz #
ssz\config.sszにさまざまな設定が書かれています。

## ジョイパッド ##
config.ssz内のin.new`[0]`.setの1番目の引数にジョイパッドの番号、
2番目以降にup,down,left,right,a,b,c,x,y,z,sの順にボタンの番号
(-1から-4は左右上下、-5から-8はハットスイッチの左右上下)

```
in.new[0].set( 
  0, -3, -4, -1, -2, //ジョイパッドの番号, 上, 下, 左, 右, 
  1, 2, 7, 0, 3, 5, //a, b, c, x, y, z, 
  9); //start 
```

2Pのキー設定はin.new`[1]`.setと書いてその引数で設定します。

## ジステージの拡大・縮小 ##
config.sszのsystemで指定したファイルでsetZoom(true)するとズームが有効になります。

# キャラクター、ステージの登録 #
script\select.luaを編集してください。

# Netplay #
テスト段階のネット対戦です。


Netplayを選択し、Input ServerにホストのIPを入力します。何も入力しないと自分がホストになります。
Escキーで切断します。