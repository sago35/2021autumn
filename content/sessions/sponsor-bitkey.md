---
key: sponsor-bitkey
title: 人生いろいろモノレポもいろいろ♪
id: sponsor-bitkey
format: conference
talkType: sponsor_session
partner: bitkey
allroom: false
speakers:
  - noriki_takahashi
videoId: EVUCSrj83uM?start=26222
---
モノレポ(Monorepo)とは、複数のモジュールやパッケージを単一のレポジトリで管理する手法です。

Go でモノレポというと最近では、Bazel (& Gazelle) を活用したものがイメージされることが多いですが、他にも実現方法はあります。
一番シンプルなものとして、単一Go モジュールによるモノレポがあります。 その他にも、ビルドツールを導入せず、Go モジュールを複数含めるパターンなど、様々なものがあります。

こうした背景をもとに発表では以下の内容をお話しします。

* モノレポの移行の目的
* モノレポが本当に必要なのか
* モノレポのどのパターンが適しているのか
* モノレポへの移行方法