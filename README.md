## LICENSE
creative commons non commercial

商用利用したい場合は twitter @sirojake にご相談ください  
please contact me for commercial use.
## developer 
ginjake

## 静電容量Helixとは？
Helix Keyboardの基板を差し替え、静電容量スイッチに対応させる為の基板です   
Varmiloスイッチ用とNizスイッチ用の2種類があり、別々の基板になっています。

## 外部の使用ライブラリ
### シンボルライブラリー
phi-kbd-library-master https://github.com/zk-phi/phi-kbd-library  
kbd https://github.com/foostan/kbd  

### フットプリントライブラリー
kbd https://github.com/foostan/kbd  
phi-kbd-library-master https://github.com/zk-phi/phi-kbd-library  
rd https://github.com/KiCad/kicad-footprints/tree/master/Resistor_SMD.pretty  
cs　https://github.com/KiCad/kicad-footprints/tree/master/Capacitor_SMD.pretty  


# 組み立て方 
本家Helixとの共通部分については省略しています。  
Varmilo版とNiz版で共通箇所が多いため、まとめて記載しています。

## 注意
本キットは組み立て難易度が高く、使うパーツも特殊です。  
自作キーボード初心者の方にはおすすめしません。  
通常のメカニカルスイッチでは動作せず、特殊なスイッチが必要になります。


## 部品

下記は両手分を作るのに必要なパーツ数です  

### 本家 Varmilo Niz共通部品
| 名前 | 数 | 備考 |
| ---- | ---- | --- |
| Pro Micro | 2個 | |
| TRRSジャック | 2個 | |
| タクトスイッチ | 2個 | |
| スプリングピンヘッダ 12P | 4個 | コンスルーとも呼ばれています |
| プレート | 2セット| 遊舎工房の切り出しサービスがおすすめです|
| OLED保護プレート | 2枚 | |
| ゴム足 | 12個 |  |
| キーキャップ | 64個 | CherryMX軸 |
| 3.5mmオーディオケーブル | 左右合わせて1本 | 左右のキーボード接続用 |
| micro USBケーブル | 左右あわせて1本 | 
| OLEDモジュール | 2個 | OLED用（オプション） |
| ピンソケット 4P | 2個 | OLED用（オプション） |
| ピンヘッダ 4P | 2個 | OLED用（オプション） |
| M2スペーサー 8mm | 4個 | (OLED用)|
| M2ネジ 3mm| 14個 | (低頭のほうが望ましい)|
| M2低頭ネジ 5mm| 4個 | |

### Niz版部品
| 名前 | 数 | 備考 |
| ---- | ---- | --- |
| M5スペーサー | 18個 | |
| M2スペーサー 7mm| 18個 | |
| M2ネジ 3mm| 36個 | |


### 本家と異なる部品
| 名前 | 数 | 備考 | 入手先 |
| ---- | ---- | --- | ---- |
| PCB | 2枚 | | |
| 静電容量キースイッチ | 64個 | 詳しくは後述します | |
| スイッチソケット | 64個 | varmilo版のみ https://yushakobo.jp/shop/a01ps/ | |
| 1608(0603)チップ抵抗 100K | 14 | | https://www.sengoku.co.jp/mod/sgk_cart/detail.php?code=EEHD-57HD |
| 1608(0603)チップ抵抗 10K | 4 | | https://www.sengoku.co.jp/mod/sgk_cart/detail.php?code=EEHD-57GX |
| 1608(0603)チップ抵抗 1KΩ | 4| | https://www.sengoku.co.jp/mod/sgk_cart/detail.php?code=EEHD-57GK |
| 1608(0603)チップ抵抗 200Ω | 12 | | https://www.sengoku.co.jp/mod/sgk_cart/detail.php?code=EEHD-57FZ |
| 1608(0603)チップ抵抗 51KΩ | 2 | | https://www.sengoku.co.jp/mod/sgk_cart/detail.php?code=EEHD-57H7 |
| 1608チップ積層セラミックコンデンサー 50Vdc 220pF | 2 | GRM1882C1H221JA01D*A (10個入り)| https://www.marutsu.co.jp/GoodsDetail.jsp?salesGoodsCode=19297&shopNo=3 |
|チップトランジスタ　2SC2712-GR 50V150m | 2 | | http://akizukidenshi.com/catalog/g/gI-00761/ |
| 74HC4051DB IC MUX/DEMUX 8X1 16SSOP | 2 | | https://www.marutsu.co.jp/pc/i/24340308/ |
| 2回路入オペアンプAD8616ARM | 2 | | http://akizukidenshi.com/catalog/g/gI-04570/ |
| ジャンパ用の銅線 | 少し | | |

### Varmilo版用キースイッチ
対応スイッチはVarmiloのECスイッチのみです。  
V1でもV2でも動作します。  

### Niz版用キースイッチ
メカニカルスイッチと異なり、複数のパーツが組み合わさって機能します。

| 名前  | 主な入手先 |
| ----  | ---- |
| 軸＆ハウジング  | https://www.nizkeyboard.com/collections/ornaments/products/2019-new-niz-ec-switch |
| ラバードーム  |  https://www.keyclack.com/products/bke-topre-dome-replacements?_pos=2&_sid=6025d869e&_ss=r もしくはREAL FORCEやNiz、HHKBから解体 |
| コニックリング | REAL FORCEやNiz、HHKB等から解体 |


## 追加で必要な工具
| 名前 | 数 | 備考 | 入手先 |
| ---- | ---- | --- | ---- |
| 絶縁テープ | 1つ | | |
| フラックス | 1つ | | |
| 拡大用ルーペ | 1つ | | |
| 懐中電灯 | 1つ | | |

## 組み立て方
右手用と左手用で若干異なります。  
写真は基本的にVarmilo版ですが、Niz版でもほぼ同じです    
Niz版とVarmilo版はスイッチ部分のフットプリントが異なるだけです。   
![image](https://user-images.githubusercontent.com/16838187/92402217-25217b00-f16a-11ea-91b9-c6515a69bad0.png)
__一度全ての工程を読み、理解してから作業を進めることをお勧めします。__

OLED,TRRSジャック等のHelixの共通部分については省略します。  
LEDについてはbacklightのみの対応です。  
(Varmilo版とNiz版で数が異なります)

## 絶縁テープとジャンパ(左手側のみ)
将来的にProMicroが刺さるところに絶縁テープを貼ります  
![image](https://user-images.githubusercontent.com/16838187/83887616-a8a28900-a783-11ea-9be4-f0edcfd9118e.png)

絶縁テープの上から、写真のようにジャンパしていきます。
この作業は左手側のみで、右手は不要です。   
![image](https://user-images.githubusercontent.com/16838187/92403955-7aab5700-f16d-11ea-92e2-cde730bb2f57.png)

ジャンパが完了したら、その上からさらに絶縁テープを貼った方が安心です。

また、絶縁テープを貼らず、ProMicro側を表裏逆転させる方法もありますが  
OLED用のスペーサーの高さが変わってしまうのであまりおすすめしません。


## その他のパーツを実装する
基板に書いてある通りにパーツを実装します。
![IMAG7291](https://user-images.githubusercontent.com/16838187/92401286-500acf80-f168-11ea-8e09-4b06152ff05c.png)

74HC4051DB　と オペアンプAD8616ARMの向きには注意してください。  
チップ側の黒い丸上の凹みと、基板上のコの時のシルクが合わさるように置くのが正解です。  
隣のピンとショートしていないか、懐中電灯で照らしながらルーペで確認しておくのがおすすめです。
![image](https://user-images.githubusercontent.com/16838187/92402159-0d49f700-f16a-11ea-9de2-8a55297e9307.png)

## リセットスイッチ
本家と同じです。

## スイッチソケットをつける(Varmilo版)
Varmilo版の場合、全てのキーにスイッチソケットをつけていきます。
![image](https://user-images.githubusercontent.com/16838187/92398487-9c9fdc00-f163-11ea-928d-3ceec87f30f6.png)


## OLEDをつける(オプション)
本家と同じです

## TRRSジャックをつける
両手分つくる場合は必要になります。  
本家と同じです


## ProMicro
本家と同じです。

## ProMicroにqmkを焼く
下記のファームウェアを焼く必要があります。  
現在はNiz版とVarmilo版は同じファームになっています。   
https://github.com/ginjake/qmk_firmware/tree/ec_helix_niz   
``make ec_helix:test:avrdude`` もしくは 
``make ec_helix:ginjake:avrdude`` 



## トッププレート
トッププレートにスペーサーをネジで固定してから、スイッチをアクリルに差込ます。  
Niz版の場合はさらに、中に軸を入れてラバードームでフタをします。  
スペーサーとラバードームが干渉しないよう、ハサミで切りましょう  
ラバードームの凹みの中にコニックリングを入れます。  
![image](https://user-images.githubusercontent.com/16838187/86467180-e937f700-bd6f-11ea-876f-b43deb603ee7.png)

このとき、コニックリングが重ね合っていないか気を付けましょう。  
複数個が重なっていても意外と気付かず、誤作動の原因になります。  


## ボトムプレート(Niz版)
基板とボトムプレートの間にM5スペーサーが入るようにネジ止めしましょう。  
この作業はVarmilo版では不要です。
![image](https://user-images.githubusercontent.com/16838187/92398269-32873700-f163-11ea-9214-1e802464c2e5.png)

## 完成
![image](https://user-images.githubusercontent.com/16838187/86467211-f81ea980-bd6f-11ea-885c-c90c43699f8e.png)


## qmkコンパイル時の諸注意
・OLEDをつけない場合は `rule.mk` の `OLED_DRIVER_ENABLE` を `no` にしてください。 
無駄な負荷がかかり、取りこぼしが発生する可能性が高くなります。   
・Varmilo版とNiz版でledの数が異なります。 `config.h` の `RGBLED_NUM` の数を適宜変更してください

・ステンレスプレートを使う場合は　`config.h` の `#define STAINLESS_PLATE` のコメントアウトを外してください。ステンレスプレートは実験的な対応の為、動作保証対象外となります。
