
#<img src="http://coffeescript.org/documentation/images/logo.png">
- CoffeeScriptとは？
- Coffeeの歴史
- CoffeeScriptの使い方
- ほかの言語との違い
- 学んでみよう！





#**CoffeeScriptとは？**
- プログラミング言語の１つでコードはJavaScriptに変換される<br>
CoffeeScriptはJavaScriptにコンパイルする言語です。
簡単に説明するとJavaScriptをRybyライクに記述できる言語に近いです。


- シンタックスシュガーの導入により、JavaScriptより簡単で読みやすい
- 配列内包やパターンマッチといった機能を追加
- 37signalsでは、実際に製品の開発に使われている
- Ruby on Rails 3.1以降 でも正式にサポートされている。





#**Coffeeの歴史**
- CoffeeScriptの始まりは「謎の言語を初回コミット(initial commit of the mystery language)」というコメントとともに Git リポジトリにコミットした
- CoffeeScriptは電子書籍である "Create Your Own Programming Language"を基に開発され、このときのコンパイラはRubyで書かれていた

#**CoffeeScriptの使い方**
CoffeeScriptは先ほど説明したようにJavaScriptに変換する言語です。
使い方はまず、```npm install -g coffee-script```でCoffeeScriptをインストールします。
そのあとCoffeeScriptで書いたテキストを```.coffee```形式で保存します。

hellp.coffee<br>
- days = [
  "Sunday"
  "Monday"
  "Tuesday"
  "Wednesday"
  "Thursday"
  "Friday"
  "Saturday"
]

today = days[(new Date).getDay()]
alert "Hello! Today is #{today}."


又は公式サイトの<br>
<img src="http://www.webopixel.net/blog/wp-content/uploads/2012/02/0213_1.png" width="500" height="300"><br>
からダウンロードしたフォルダのcoffee-script.js



#**コンパイルしてみる**
- CoffeeScriptをJavaScriptにコンパイルするとこのようになります。
- ver宣言

|CoffeeScript|JavaScript|
|:-----------|:---------|
|num = 3245|(function() {|
|console.log num|var num;|
||num = 3245;|
||console.log(num);|
||}).call(this);|

- for文

|CoffeeScript|JavaScript|
|:-----------|:---------|



- if文

|CoffeeScript|JavaScript|
|:----------|:--------|
||var footprints, solipsism, speed;|
|solipsism = true if mind? and not world?|if ((typeof mind !== "undefined" && mind !== null) && (typeof world === "undefined" ｜｜ world === null)) {solipsism = true;}|
|speed = 0|speed = 0;|
|speed ?= 15|if (speed == null) {speed = 15;}|
|footprints = yeti ? "bear"|footprints = typeof yeti !== "undefined" && yeti !== null ? yeti : "bear";|





#学んでみよう！
- CoffeeScriptの公式ページ
- CodeCombatでCoffeeScriptを使って遊ぶ
