# Carduino

![omote](Carduino_v20_1.jpg)

Carduinoは、クレジットカードサイズ・厚さ2.4mmの、Arduino互換機(ArduinoProMini/8MHz)です。
財布などにいつもいれておいて、いつでもその場でArduinoを使うことができます。
「Arduinoは興味あるんだけど、まだ触ったことないんだよね」という人に会ったら、その場でArduinoを体験してもらいましょう。
* ArduinoIDEの導入からLチカまでの手順は、本体裏面にシルクで書かれています。またArduinoIDEのダウンロード先もQRコードで読み取れます。
* USB-Aコネクタ（収納式）で、PCのUSB端子に直接差し込むことができます。またmicroUSBケーブルで接続することもできます。
* Arduinoの入出力端子はメスソケットですので、ジャンパワイヤ等をさしてつかうこともできます。
* USB-シリアル変換には、FTDI FT232Rを使っています。
* [スイッチサイエンスで委託販売はじまりました](https://www.switch-science.com/catalog/3917/)

![ura](Carduino_v20_2.jpg)

# 使い方

本体裏面のシルクを参照してください。

PCとの接続は、以下の2通りが可能です。
* 本体のコネクタをいったんはずし、以下のようにとりつけ、PCのUSBポートに直接さしこみます。（※コネクタの向きに注意してください。表裏が逆の場合、本体やPCを破損する恐れがあります）
![USB connector](Carduino_v20_conn.jpg)

* microUSBケーブルを以下のように本体にさしこみます。（表裏に注意してください。基板パターンがある面が、ケーブルのmicroUSBコネクタの端子側になります） 

![microUSB connector](Carduino_v20_uUSB.jpg)

なお未使用時にUSBコネクタ部を格納しておくコネクタには、A6/A7、電源5V、GNDがつながっています。

# 作り方

* ガーバーデータ(Carduino_v20_gerber.zip)で基板製造（板厚1.0mm）し、BOM（部品表）の部品をとりつけます。※v20は、D0-D7のコネクタ用の基板切り書きの位置が少し間違っています。基板を少し削れば取り付け可能ですが、気になる場合は修正版ガーバーデータ(Carduino_v21_gerber.zip)を使用してください。ただし後述のレーザー加工データを少し修正する必要があります（未修正）
* 4p、6p、8pのピンソケット（各2個：秋月電子等で購入できます）を、基板の溝にあわせて横向けにはんだ付けします。また4pピンヘッダ（秋月電子等で購入できます）をUSBコネクタ側にとりつけます。
* microUSBコネクタ部を使用する場合は、コネクタ部周辺をフライス盤で、板厚0.6mmまで削ります
* 板厚1mmのアクリル板をレーザーカッター等でカットし、本体に透明両面テープや木工用ボンド等で固定します。
* ArduinoProMini(3.3V,8MHz)用のブートローダを書き込みます

# 作者

Junichi Akita (akita@ifdl.jp, @akita11)

