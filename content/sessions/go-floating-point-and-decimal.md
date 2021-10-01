---
key: go-floating-point-and-decimal
title: Floating Point Numbers and Decimal in Go
id: go-floating-point-and-decimal
format: conference
talkType: ""
allroom: false
speakers:
- sekino_pii
---
プログラミングにおける小数の扱いは、注意が必要な定番のポイントだと思います。特に、精緻な計算が必要な処理では、桁落ちやオーバーフローを考慮することになります。

Goでは、組み込みの型の小数の挙動に少し独特な部分があります。また、精緻な計算を要求される場面では、math/bigパッケージなど、細かい小数を扱う仕組みも標準で提供されています。

そこでこのセッションでは、Goの組み込みの文法での小数の挙動を実際に見た上で、汎用的なアプローチとして、公式のmath/bigやサードパーティーのshopspring/decimalパッケージを利用した小数の取り扱い方法を紹介したいと思います。

---

# ゴール

- Goの組み込みの文法の小数の挙動がわかること
- Goで小数を含む精緻な計算をする際に、注意すべき点や実際のアプローチ例がわかること

# 話す予定のトピック

- プログラミングにおける小数 (前提確認)
- floatの小数の扱い
- untypedな定数の小数の扱い
- math/bigパッケージを使用した実装
- shopspring/decimalパッケージを使用した実装