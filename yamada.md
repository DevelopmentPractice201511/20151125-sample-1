
#<img src="http://coffeescript.org/documentation/images/logo.png">
- CoffeeScriptとは？
- CoffeeScriptの使い方
- ほかの言語との違い
- 学んでみよう！


#**CoffeeScriptとは？**
- プログラミング言語の１つでコードはJavascriptに変換される
- シンタックスシュガーの導入により、JavaScriptより簡単で読みやすい
- 配列内包やパターンマッチといった機能を追加

シンタックスシュガーとは、プログラミング言語の読み書きのしやすさのために、既に存在する構文に別の記法を与えたもの。 

これにより、パフォーマンスを下げることなく、より短いコードでプログラムを記述することができる 
2011年3月16日から一時的に、CoffeeScript は GitHub でもっとも閲覧されているプロジェクトだった

この言語はRubyコミュニティによく受け入れられており、37signalsでは、実際に製品の開発に使われている
Ruby on Rails 3.1以降 でも正式にサポートされている。

「JavaScript の未来」に影響を与えたものとして CoffeeScript に言及している

#**Coffeeの歴史**
CoffeeScriptの始まりは「謎の言語を初回コミット(initial commit of the mystery language)」というコメントとともに Git リポジトリにコミットした
CoffeeScriptは電子書籍である "Create Your Own Programming Language"を基に開発され、このときのコンパイラはRubyで書かれていた

同年12月24日には初めてタグとドキュメントのついた、バージョン 0.1.0 がリリースされた。2010年2月21日には、コンパイラを純粋な CoffeeScript で記述した、バージョン 0.5 がコミットされる。この頃にはこのプロジェクトは GitHub を利用する他の開発者の興味を引き、1日に300回ほどプロジェクトページが参照された。 2010年12月24日 Askenas は、安定版であるバージョン 1.0.0 のリリースを、Hacker News で発表した[9]。 なお、Hacker News は、最初のバージョンを発表した場でもある

#**他の言語との違い**
- 演算子

|Coffee                           |Java                               |
|:--------------------------------|:----------------------------------|
|                                 |var modulo = function(a, b) { return (+a % (b = +b) + b) % b; };|
|-7 % 5 == -2                     |-7 % 5 === -2;                     |
|-7 %% 5 == 3                     |modulo(-7, 5) === 3;               |
|tabs.selectTabAtIndex((tabs.currentIndex - count) %% tabs.length)|tabs.selectTabAtIndex(modulo(tabs.currentIndex - count, tabs.length));|

|Coffee                           |Java                               |
|:--------------------------------|:----------------------------------|
|                                 |var footprints, solipsism, speed;  |
|solipsism = true if mind? and not world?|if ((typeof mind !== "undefined" && mind !== null) && (typeof world === "undefined" || world === null)) {solipsism = true;}|
|speed = 0                        |speed = 0;                         |
|speed ?= 15                      |if (speed == null) {speed = 15;}   |
|footprints = yeti ? "bear"       |footprints = typeof yeti !== "undefined" && yeti !== null ? yeti : "bear";|
#学んでみよう！
CoffeeScript
CodeCombatではCoffeeを使って遊ぶ事が出来ます
