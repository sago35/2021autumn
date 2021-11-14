---
key: go-floating-point-and-decimal
title: Floating Point Numbers and Decimal in Go
id: go-floating-point-and-decimal
format: conference
talkType: ""
allroom: false
speakers:
- sekino_pii
videoId: EVUCSrj83uM?start=23229
slides: https://speakerdeck.com/sryoya/floating-point-numbers-and-decimal-in-go
---
プログラミングにおける小数の扱いは、注意が必要な定番のポイントだと思います。特に、精緻な計算が必要な処理では、桁落ちやオーバーフローを考慮することになります。

Goでは、組み込みの型の小数の挙動に少し独特な部分があります。また、精緻な計算を要求される場面では、math/bigパッケージなど、細かい小数を扱う仕組みも標準で提供されています。

そこでこのセッションでは、Goの組み込みの文法での小数の挙動を実際に見た上で、汎用的なアプローチとして、公式のmath/bigやサードパーティーのshopspring/decimalパッケージを利用した小数の取り扱い方法を紹介したいと思います。
