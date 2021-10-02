---
key: io-fs-fs-testability-abstraction
title: io/fs.FS for testability. io/fs.FS for abstraction.
id: io-fs-fs-testability-abstraction
format: conference
talkType: ""
allroom: false
speakers:
- k1low
---
Go 1.16から追加されたio/fsパッケージが提供しているインターフェースについて、皆さんはどのような目的で活用していますか？

私は、主に2つの目的で活用しています。1つはテスト容易性（テスタビリティ）、もう1つはファイルシステムとしての抽象化です。

本発表では、具体的な事例を元に上記の2つの目的での使い方を紹介します。
また、fs.FSインターフェースを使ったことで失敗した事例も紹介したいと思います。

本発表を通じてio/fsのインターフェースの利用イメージを持ってもらえれば嬉しいです。