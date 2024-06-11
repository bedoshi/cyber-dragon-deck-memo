# サイバー・ドラゴンデッキ
## はじめに
どっからでも相手のライフを直葬できる出力の高さが売りの後攻ワンキルが狙えるデッキ。<br>起点になるのは小粒の「俺サイバー・ドラゴンっす」なカード達。もともと「サイバー」と名前のついたカードであるため、豊富なサポートカードからサーチが可能であり、サイバー・ドラゴンであれば融合の起点になることを忘れずにいよう。

特に《キメラテック・フォートレス・ドラゴン》や《キメラテック・メガフリート・ドラゴン》のように融合を必要とせず、相手の機械族モンスターを巻き込みながら融合召喚することで、相手の盤面を壊してライフを直接削りに行ける仕組みがほんっっっっっっとうに強い。

「相手が機械族デッキじゃなかったらこの強みってなくない？？」

そんな声が聞こえてきそうだが、《機械仕掛けの夜-クロックワークナイト》がすべてを解決してくれる。

あと以降のやつは[タクティカルトライデッキのリスト](https://www.yugioh-card.com/japan/products/tt01a/)を前提としている。
## 起点になりそうなカード
### サイバー・ドラゴン・コア
|イラスト|効果|
|---|---|
|![サイバー・ドラゴン・コア](https://storage.googleapis.com/gachi-matome.appspot.com/1/card100015531_1-10.jpg)|星２/光属性/機械族/攻 400/守1500<br>このカード名の②③の効果は１ターンに１度、いずれか１つしか使用できない。<br>①：このカードのカード名は、フィールド・墓地に存在する限り「サイバー・ドラゴン」として扱う。<br>②：このカードが召喚に成功した場合に発動する。<br>デッキから「サイバー」魔法・罠カードまたは「サイバネティック」魔法・罠カード１枚を手札に加える。<br>③：相手フィールドにのみモンスターが存在する場合、墓地のこのカードを除外して発動できる。<br>デッキから「サイバー・ドラゴン」モンスター１体を特殊召喚する|

このカードができることは以下の通り。
- サイバー・ドラゴンとして扱えること。
  - サイバー・ドラゴンであることから、機械複製術でデッキからサイバー・ドラゴン2体をSSできる。
- ETBでサイバー/サイバネティック魔法罠をサーチできること。
- 相手のモンスターのみが存在する場合に墓地から除外することでサイバー・ドラゴンをSSできること。

ここまでで言えることをまとめるとこんな感じ。
```mermaid
flowchart TD

subgraph "サイバー・ドラゴン・コア"
a1[通常召喚]-->a2[着地効果が誘発]
a2-->|墓地にサイバー・ドラゴンがある|a3[サイバー・リペア・プラント]
a3-->a4[墓地からサイバー・ドラゴンをリアニ]
a3-->a5[墓地から光属性機械族をデッキに戻す]
a2-->|手札・墓地からサイバー・ドラゴンを出したい|b1[サイバー・レヴシステム]
a2-->|デッキからカードをサーチしたい|c1[エマージェンシー・サイバー]
a2-->|パワー・ボンドがほしい|d1[サイバー・ダーク・ワールド]
d1-->|サイバー・ダーク召喚効果起動|d2[サイバー・ダーク・キメラ召喚]-->d3[パワー・ボンドサーチ]
end
```
```mermaid
flowchart TD

subgraph "サイバー・ドラゴン・コア着地後"
d1[機械複製術]-->|サイバー・ドラゴンとして処理|d2[サイバー・ドラゴン2体をデッキからSS]
d2-->|パワー・ボンドがある|d3[融合召喚]
d3-->|8000で守備貫通攻撃|d4[サイバー・エンド・ドラゴン]
d3-->|5600で2回攻撃|d5[サイバー・ツイン・ドラゴン]
d2-->|クロックワークナイトがある|e1[キメラテック~~??（サイバー・ドラゴン1体と相手のモンスターで融合）]
e1-->|相手のExデッキから出たやつを全部食う|e2[メガフリート・ドラゴン]
e1-->|相手のモンスターなら何でも食う|e3[フォートレス・ドラゴン]
end
```
あとフィールドと墓地にいるときは①の効果でサイバー・ドラゴンとして扱えるので、キメラテック・ランページやらのコストにできたり、サイバー・ドラゴン・ズィーガーを出すためのリンク素材になったりもする（本当に重要）。

### エマージェンシー・サイバー
|イラスト|テキスト|
|---|---|
|![エマージェンシー・サイバー](https://m.media-amazon.com/images/I/51gVqerffTL._AC_UF894,1000_QL80_.jpg)|このカード名のカードは１ターンに１枚しか発動できない。<br>①：デッキから「サイバー・ドラゴン」モンスターまたは通常召喚できない機械族・光属性モンスター１体を手札に加える。<br>②：相手によってこのカードの発動が無効になり、このカードが墓地へ送られた場合、手札を１枚捨てて発動できる。このカードを手札に加える。|

大体うららが飛んでくるカード筆頭候補（コアよりもこっちに飛んでくるイメージ）。基本的に以下の3卓ぐらいになる。
1. サイバー・ドラゴン・コア: 最優先のサーチ先。
2. サイバー・ドラゴン・ヘルツ: 手札にコアが存在する状況かつ銀河戦士が手札にあるときのコストにするとサイバー・ドラゴンをサーチできて手札ロスが発生しない。
3. サイバー・ドラゴン: 後攻展開でコアが手札にあるとき、最初のSSに使ったり。

ざっくりまとめるとこれか。
```mermaid
flowchart TD

subgraph "エマージェンシー・サイバー"
a1[エマージェンシー・サイバー]
a1-->|手札にコアがないならとりあえず選ぶ|a2[サイバー・ドラゴン・コア]
a1-->|手札にコアと銀河戦士を持っている|a3[サイバー・ドラゴン・ヘルツ]
a1-->|後手かつコアが手札にあるケース|a4[サイバー・ドラゴン]

a2-->b1[サイバー・ドラゴン・コアの展開ルートへ]
a3-->c1[ヘルツをコストに銀河戦士を特殊召喚]-->c2[デッキから銀河戦士をサーチ]
c1-->|ヘルツが墓地に落ちた時誘発|c11[サイバー・ドラゴンをサーチ]
c11-->c2-->|ヘルツからサーチしたのをコストにする|c3[銀河戦士２枚目を特殊召喚]
c3-->|銀河戦士2枚でXYZ|c4[サイバー・ドラゴン・ノヴァをXYZ]
c4-->|サイバー・ドラゴン・ノヴァの①を起動|c5[墓地からサイバー・ドラゴンを特殊召喚]-->c6[サイバー・ドラゴン・インフィニティを重ねてXYZ]
c6-->|相手の盤面にカードがあれば|c7[インフィニティ起動で相手のカードをXYZ化する]
c7-->c8[なんでも1妨害]
c8-->c9[サイバー・ドラゴン・コアの展開ルートへ]
a4-->|融合素材の数+1として|d1[サイバー・ドラゴン・コアの展開ルートへ]
end
```

## 参考文献
1. 遊戯王OCGデュエルモンスターズ TACTICAL-TRY DECK 終撃竜サイバー・ドラゴン | 商品情報 - https://www.yugioh-card.com/japan/products/tt01a/
1. 遊戯王カードwiki - https://yugioh-wiki.net/
1. 遊戯王 オフィシャルカードゲーム デュエルモンスターズ - カードデータベース - https://www.db.yugioh-card.com/yugiohdb/
