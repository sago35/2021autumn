---
key: go-static-analysis
title: Goで静的解析をはじめてみよう
id: go-static-analysis
format: conference
talkType: ""
allroom: false
speakers:
- d_tutuz
---
静的解析を行うことで、プログラムの品質を高めることができます。Goでは `golang.org/x/tools/go/analysis` というパッケージを用いることによって、静的解析にあまりなじみがない開発者も、字句解析や構文解析を自前で実装せずに、静的解析モジュールを実装できます。

本LTでは、静的解析のモジュールを作った私の経験をもとに、静的解析のモジュール実装が身近なものであることをお伝えします。本LTのリスナーが静的解析のモジュールが実装できるんだ、と思ってもらえることをゴールとします。

---

静的解析はプログラムのバグを早期に検出し、品質向上に寄与します。Goでは `golang.org/x/tools/go/analysis` パッケージを用いることで、構文解析や字句解析をモジュール開発者自身が実装することなく、静的解析で検出したいロジックに注力できます。

`golang.org/x/tools/go/analysis` パッケージを用いて静的解析モジュールを自作した経験から、Goで静的解析を始める方法をお伝えします。