# __windows_trick__

## プログラムの目的
ウィンドウを活用したサプライズや，遊び心の演出に使用できます．また，このプログラムによって発生したトラブルについては一切の責任を負いません．自己責任でご利用ください．

## 実行方法
プログラムの実行にはTkinterを必要とします．TkinterとはPythonに標準搭載されているGUIライブラリであり，インストールされていない場合は以下のコマンドを打ち込んだ後に本プログラムを使用してください．
```
$ sudo apt-get install python3-tk
```
プログラムの実行に伴い，プログラム終了に必要なボタンのクリック数も入力します．必ず正の整数を使用して下さい．
```
$ git clone https://github.com/OMame06/windows_trick.git
```
```
$ cd windows_trick
```
```
$ echo <number>| ./pesky_windows
```

## プログラム概要
### 実行結果
プログラムを実行することでボタンが付いたウィンドウが１枚表示されます．ボタンをクリックするとウィンドウが増えていきます．ボタンの数はクリックした回数に応じて増えていきます．ウィンドウを閉じようと右上のバツ印を押してもボタンを押したときと同様の結果を得られます．また，バツ印を押した場合「追加ウィンドウの上限」が１枚増加します．ウィンドウを削除する為には標準入力した数値の分だけボタンをクリックする必要があります．クリックするウィンドウに指定はありません．
### 追加ウィンドウの上限
ユーザーによる押し間違いを考慮して，増えるウィンドウの枚数には上限が設定されています．初期設定では10枚となっている為，必要に応じて値を変更してください．
### 標準入力される数値
正の整数のみ読み取る事が出来ます．負の整数を入力した場合，打ち間違いと判断されて符号が変換されたのちプログラムの実行に移ります．数値でない値，整数ではない値を入力した場合はエラー文が表示されます．

## 必要なソフトウェア
- Python
  - テスト済みバージョン: 3.7~3.11

## テスト環境
- Ubuntu 22.04.5 LTS
  
## ライセンス
このソフトウェアパッケージは，3条項BSDライセンスの下，再頒布および使用が許可されます．

© 2024 Kinjo Riku
