
#<img src="http://coffeescript.org/documentation/images/logo.png">
- CoffeeScriptとは？
- Coffeeの歴史
- CoffeeScriptの使い方
- ほかの言語との違い
- 学んでみよう！





#**CoffeeScriptとは？**
- プログラミング言語の１つでコードはJavascriptに変換される
- シンタックスシュガーの導入により、JavaScriptより簡単で読みやすい
- 配列内包やパターンマッチといった機能を追加
- 37signalsでは、実際に製品の開発に使われている
- Ruby on Rails 3.1以降 でも正式にサポートされている。





#**Coffeeの歴史**
- CoffeeScriptの始まりは「謎の言語を初回コミット(initial commit of the mystery language)」というコメントとともに Git リポジトリにコミットした
- CoffeeScriptは電子書籍である "Create Your Own Programming Language"を基に開発され、このときのコンパイラはRubyで書かれていた





#**他の言語との違い**
- 演算子

|Coffee                           |Java                               |
|:--------------------------------|:----------------------------------|
|                                 |var modulo = function(a, b) { return (+a % (b = +b) + b) % b; };|
|-7 % 5 == -2                     |-7 % 5 === -2;                     |
|-7 %% 5 == 3                     |modulo(-7, 5) === 3;               |
|tabs.selectTabAtIndex((tabs.currentIndex - count) %% tabs.length)|tabs.selectTabAtIndex(modulo(tabs.currentIndex - count, tabs.length));|

- if文

|Coffee                           |Java                               |
|:---------------------------------------|:----------------------------------|
|                                 |var footprints, solipsism, speed;  |
|solipsism = true if mind? and not world?               |if ((typeof mind !== "undefined" && mind !== null) && (typeof world === "undefined" ｜｜ world === null)) {solipsism = true;}|
|speed = 0                        |speed = 0;                         |
|speed ?= 15                      |if (speed == null) {speed = 15;}   |
|footprints = yeti ? "bear"       |footprints = typeof yeti !== "undefined" && yeti !== null ? yeti : "bear";|





#学んでみよう！
- CoffeeScriptの公式ページ
- CodeCombatでCoffeeScriptを使って遊ぶ
