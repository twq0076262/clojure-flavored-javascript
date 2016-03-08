# 1 前言

函数式编程可以说是非常古老的编程范式， 但是近年来函数式编程越来越受到关注。不管是 Google 力推的 Go, 学术派的 Scala 与 Haskell，还是 lisp 跑在 JVM 上的新方言 Clojure，这些新的函数式编程语言也都越来越受到关注。

当然不仅是后端函数式语言层出不穷，前端也不甘示弱。 即便前端浏览器只支持一门语言——JavaScript，但是 能支持函数式编程的 JavaScript 库越来越多，比如 Functional JavaScript，Underscore, lodash…不仅如此， 还有一些能编译成 JavaScript 的语言，能让前端的函数式编程发挥到极致, Haskell 的 PureScript, Scala 的 scalajs, Clojure 的 ClojureScript。

我两次都以 Clojure 结尾，是因为我喜欢把重点的留到最后。 Clojure 独特于其他的语言，它即是一门新的语言， 一门函数式编程范式的语言，同时又流淌着着古老的lisp血液。 这是我选择用 Clojure 来诠释函数式编程的原因之一。

那么为什么我要选 JavaScript 作为函数式编程的目标呢。首先，正如 Rich Hickey 所言——“Clojure is Awesome, but JavaScript reaches”。Michael Fogus 用二百多页向大家展示了不一样的《Functional JavaScript》编程方式， 可惜 Fogus 作为 ClojureScript 编译器的贡献者， 竟然选择了 Underscore 作为函数式库， 直接导致并不能完全展示 JavaScript 所能达到的函数式编程能力。有趣的是， ClojureScript 的作者把 ClojureScript 的不可变（Immutable）数据结构移植到了 JavaScript, 这下彻底将 JavaScript 的函数式编程提升到了用其他库都完成不了的新高度（虽然 facebook 也尝试实现自己的一个不可变数据结构 Immutable.js）。 不仅如此, Mozilla 的 Sweet.js（https://github.com/mozilla/sweet.js） 更是完成了另一个突破 —— JavaScript 的 macro， 虽然不能算是函数式的概念，但也算是 lisp 语言的一项独门绝技了（虽然很多新的语言都在 尝试实现 macro，比如 scala, rust 和 julia，但是由于语法过于复杂）。

这一切的一切，都让我忍不住要帮 Fogus 出一本续集，用 JavaScript 实现其他函数式编程语言如 Clojure 甚至是 Haskell（就当是bonus了）的奇淫巧技， 让大家进一步感受用 JavaScript 这门不完美的语言， 同样可以编写出优雅的函数式代码，以不一样的方式思考和解决问题。 于是不管你是想转行 JavaScript 的 Clojure 开发者， 亦或是像了解 Clojure 或函数式编程的 JavaScript 开发者, 都可以在此找到一些启发。 但这并不是一本 JavaScript 入门的好书（Douglas 的《JavaScript 语言精粹》 是个不错的选择。另外如果读者的英文好的话，还有一本可以在线免费阅读的[https://leanpub.com/javascriptallongesix/read](《JavaScript Allonge》)）。