# GasByKotlin

GASをKotlin1.4で動かしてみたサンプルです

# ディレクトリ構造
- gas
  - GASで動かしたいJSのコードが含まれます。現状のKotlin/JSの性質上、GASとKotlin/JSによって出力されたJavaScriptとのグルーとなる箇所が必須となり、この部分にその処理を書く事になります
- gas_dist
  - browserifyの出力をここに設定し、`clasp push`でGASにpushするためのディレクトリです
- src
  - Kotlinのコードが含まれます
  
# 使い方
1. Kotlinのコードを書く
2. Kotlinのコードをビルドする
3. gas/main.jsを書く
4. `./gradlew buildAndPush`