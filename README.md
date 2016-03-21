# Flmml vs SiON

現状、flmmlはhtml5版が存在し、OPMエミュレーションも実現されている。
音源の仕様上、文法が異なる箇所もあるため、ラッパーを作れないか検討する。

http://carborane3.github.io/FlMMLonHTML5/

# 気づいたこと

 * 実はOPM音色指定ができるが、UNDOCUMENTED？
  * カンマありでも食べてくれるみたい
 * %6 @0形式から@14-0形式への変換が必要
 * FMチャンネルだけ随分音量が違う。v8 -> v12ぐらいにするとちょうどいい。
  * 音量の解釈が違う？変換テーブルが必要かも。
  * 内部のFMGenの影響か？
 * flmml workerは実行パスに置く必要がある。

# 雰囲気

 * FMチャンネルのみコンバートが必要な雰囲気
 * 利用コマンドを制限すればある程度使えそう
