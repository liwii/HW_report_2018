# ハードウェア構成法 冬休み特訓レポート2018

皆さんに宿題を手伝ってもらいたくてリポジトリを作りました。PRくれる優しい人がいると泣いて喜びます・・・
MacでGHDLを使って開発してます。  
[GHDL on OS X](http://lv4.hateblo.jp/entry/2015/01/26/090928)  
[GHDL](http://ghdl.free.fr/)

## 問題
> 10ビットの正数 : 変域 1~1023 について, 偶数なら2で割る 奇数なら3倍して+1する を繰り返していると, 数字が大小を繰り返しそのうち1になります. これを Collatz 山脈と呼ぶことにします. Collats 山脈の最高峰を与える登り口 (=奇数) のうち 最も行程の長いスタート地点の数字をルートの名前とします. 例えば 7, 8, 9, 10, 11 からスタートした場合 最高峰は52になりますが行程の一番長い9をルート名とします. 最高峰が高い順に上位4本のルート名とその行程の長さを計算する回路を設計してください.

## 変更履歴

### v1
与えられた数でCollatz山脈を上り下りした時の
- 最高峰
- ルートの長さ
  
を出力する`Collatz`を実装しました。`collatz_tb.vhd`を走らせると、1~1023で走らせた結果をレポートします。