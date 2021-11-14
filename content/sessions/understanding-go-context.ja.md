---
key: understanding-go-context
title: Go Contextを完全に理解する
id: understanding-go-context
format: conference
talkType: ""
allroom: false
speakers:
- it_guitar
videoId: EVUCSrj83uM?start=11862
slides: https://www.slideshare.net/ssuserebd24d1/go-conference-2021-autumn-context
---
Goではcontext.Contextを利用することで、キャンセルやタイムアウトを効率よく安全に実装することができます。
ContextはDBクライアントなど各種ライブラリを使う際に、対応する関数の引数にするだけでも動作します。
Contextはとても抽象度の高い存在ですが、実体はわずか数百行のコードで完結したライブラリです。
それだけの行数で動作するよう、非同期処理、インターフェースが高度に実装されています。
詳細な実装まで読み解いて、Contextをしっかりと理解してみたくなりませんか。