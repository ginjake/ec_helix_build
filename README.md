## 静電容量Helixとは？
Helix Keyboardの基板を差し替え、静電容量スイッチに対応させる為の基板です   
Varmiloスイッチ用とNizスイッチ用の2種類があり、本リポジトリはNiz版です

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
本家Helixとの共通部分については省略しています

## 注意
本キットは組み立て難易度が高く、使うパーツも特殊です。  
自作キーボードについて、最低限の知識があることを前提にドキュメントを書いています  
Varmilo対応版と、niz対応版で基板が異なりますが、組み立て方はほぼ同じです。  
通常のメカニカルスイッチでは動作しません

## 部品

下記は両手分を作るのに必要な部品の数です。
### 本家と共通の部品
| 名前 | 数 | 備考 |
| ---- | ---- | --- |
| Pro Micro | 2個 | |
| TRRSジャック | 2個 | |
| タクトスイッチ | 2個 | |
| スプリングピンヘッダ 12P | 4個 | コンスルーとも呼ばれています |
| プレート（アクリル） | 2セット| |
| 保護プレート | 2枚 | |
| M2スペーサー 7mm| 12個 | |
| M2スペーサー 8mm | 4個 | (OLED用)|
| M2ネジ 3mm| 28個 | (低頭のほうが望ましい)|
| M2低頭ネジ 5mm| 4個 | |
| ゴム足 | 12個 |  |
| キーキャップ | 64個 | キースイッチと互換があるもの |
| 3.5mmオーディオケーブル | 左右合わせて1本 | 左右のキーボード接続用 |
| micro USBケーブル | 左右あわせて1本 | 
| OLEDモジュール | 2個 | OLED用（オプション） |
| ピンソケット 4P | 2個 | OLED用（オプション） |
| ピンヘッダ 4P | 2個 | OLED用（オプション） |


### 本家と異なる部品
| 名前 | 数 | 備考 | 入手先 |
| ---- | ---- | --- | ---- |
| PCB | 2枚 | | |
| 静電容量キースイッチ | 64個 | 詳しくは後述します | |
| 1608(0603)チップ抵抗 100K | 16 | | https://www.sengoku.co.jp/mod/sgk_cart/detail.php?code=EEHD-57HD |
| 1608(0603)チップ抵抗 10K | 4 | | https://www.sengoku.co.jp/mod/sgk_cart/detail.php?code=EEHD-57GX |
| 1608(0603)チップ抵抗 1KΩ | 4| | https://www.sengoku.co.jp/mod/sgk_cart/detail.php?code=EEHD-57GK |
| 1608(0603)チップ抵抗 200Ω | 12 | | https://www.sengoku.co.jp/mod/sgk_cart/detail.php?code=EEHD-57FZ |
| 1608チップ積層セラミックコンデンサー 50Vdc 220pF | 2 | GRM1882C1H221JA01D*A (10個入り)| https://www.marutsu.co.jp/GoodsDetail.jsp?salesGoodsCode=19297&shopNo=3 |
|チップトランジスタ　２ＳＣ２７１２－ＧＲ　５０Ｖ１５０ｍ | 2 | | http://akizukidenshi.com/catalog/g/gI-00761/ |
| 74HC4051DB IC MUX/DEMUX 8X1 16SSOP | 2 | | https://www.marutsu.co.jp/pc/i/24340308/ |
| ２回路入オペアンプＡＤ８６１６ＡＲＭ | 2 | | http://akizukidenshi.com/catalog/g/gI-04570/ |
| ジャンパ用の銅線 | 少し | | |
| M2スペーサー 8mm | 12個 | 西川電子部品など |
| ゴム足 | 追加で8個 | 遊舎工房の店頭など |
| ワッシャー | 適宜 | M2用 |
  
### キースイッチ
メカニカルスイッチと異なり、複数のパーツが組み合わさって機能します。

| 名前  | 主な入手先 |
| ----  | ---- |
| 軸＆ハウジング  | https://www.nizkeyboard.com/collections/ornaments/products/2019-new-niz-ec-switch |
| ラバードーム  |  https://www.keyclack.com/products/bke-topre-dome-replacements?_pos=2&_sid=6025d869e&_ss=r　もしくは中古のREAL FORCE |
| コニックリング | 中古のREAL FORCE等 |


## 追加で必要な工具
| 名前 | 数 | 備考 | 入手先 |
| ---- | ---- | --- | ---- |
| ヒートクリップ | 1つ | | |
| カプトンテープ | 1つ | | 絶縁テープでも可|
| フラックス | 1つ | | |
| 温度調節機能のついたハンダコテ | 1つ | | |

## 組み立て方
以降は右手用で説明します。左手用はPCBを反転して下さい。  
写真は基本的にVarmilo版ですが、Niz版でもほぼ同じです    
Niz版は次のように、スイッチ部分のフットプリントが異なるだけです   
![image](https://user-images.githubusercontent.com/16838187/86467118-ca396500-bd6f-11ea-833a-8518ff53b99a.png)  
__一度全ての工程を読み、理解してから作業を進めることをお勧めします。__

OLED,TRRSジャック等のHelixの共通部分については省略します。
LEDについてはunderglow、backlight共に未対応です

## 最初に絶縁テープを貼る
将来的にProMicroが刺さるところに絶縁テープを貼ります  
![image](https://user-images.githubusercontent.com/16838187/83887616-a8a28900-a783-11ea-9be4-f0edcfd9118e.png)

## 左右をジャンパ
絶縁テープの上から、写真のようにジャンパしていきます  
![image](https://user-images.githubusercontent.com/16838187/83893604-1d2cf600-a78b-11ea-9552-fb847786772a.png)

## 絶縁テープ
ジャンパの上に絶縁テープを貼ります  
![image](https://user-images.githubusercontent.com/16838187/83893829-73019e00-a78b-11ea-98b6-a781e42b639f.png)

## 裏側に各種パーツを実装する
基板をひっくり返し、各種パーツを実装します  
74HC4051DB　と オペアンプAD8616ARMの向きには注意してください。    
また、熱に弱いためヒートクリップ等を使うことをおすすめします。   
温度調節機能付きハンダコテの場合は300度以下にしたほうがよいかもしれません。
![ポンチ図](https://user-images.githubusercontent.com/16838187/87218828-4ac01d00-c391-11ea-9f25-194563ae06af.png)

## その他のパーツを実装する
下記画像のパーツを実装していきます。  
![ポンチ図2](https://user-images.githubusercontent.com/16838187/83897147-29678200-a790-11ea-98a0-5f82ccec384a.png)  
![ポンチ図3](https://user-images.githubusercontent.com/16838187/83898727-443af600-a792-11ea-9359-abdeb232eadb.png)  



## リセットスイッチ
本家と同じです。


## OLEDをつける(オプション)
本家と同じです  
(この写真では、家にあった適当なタクトスイッチを代用したので、OLED保護プレートと干渉してます。


## TRRSジャックをつける
両手分つくる場合は必要になります。  
本家と同じです


## ProMicro
本家と同じです

## ProMicroにqmkを焼く
下記のファームウェアを焼く必要があります  
https://github.com/ginjake/qmk_firmware/tree/ec_helix_niz  
``make ec_helix:ginjake:avrdude``

## トッププレート
スイッチをアクリルに入れ、中に軸を入れてラバードームでフタをします。  
スペーサーとラバードームが干渉しないよう、ハサミで切ります。  
ラバードームの凹みの中にコニックリングを入れます  
![image](https://user-images.githubusercontent.com/16838187/86467180-e937f700-bd6f-11ea-876f-b43deb603ee7.png)

このとき、コニックリングが重ね合っていないか気を付けましょう。
複数個が重なっていても意外と気付かず、誤作動の原因になります。  


## ボトムプレート
外側だけでなく、内側にもゴム足を装着します。  
これがないと、チップ部品がアクリルと基板を支える事になり、タイピングの力が直接かかります。  
![image](https://user-images.githubusercontent.com/16838187/86486254-c15b8a00-bd95-11ea-9f22-722668908eff.png)  
![image](https://user-images.githubusercontent.com/16838187/86486365-0ed7f700-bd96-11ea-810b-874c11bce676.png)
ワッシャーを適宜(2枚程度)入れたあと、7mmスペーサーをネジ止めします。
内側のゴム足の高さによって、必要な枚数が異なる可能性があります。

## サンドイッチ
トッププレートと基板とボトムプレートをサンドイッチし、ネジで固定します  
隙間が空かない用、ぎゅっと押し込みましょう
実際に打ってみて、問題なさそうなら完成です
![image](https://user-images.githubusercontent.com/16838187/86467211-f81ea980-bd6f-11ea-885c-c90c43699f8e.png)
