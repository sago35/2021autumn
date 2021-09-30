---
key: understanding-go-context
title: Go Contextを完全に理解する
id: understanding-go-context
format: conference
talkType: ""
allroom: false
speakers:
- it_guitar
---
Goではcontext.Contextを利用することで、キャンセルやタイムアウトを効率よく安全に実装することができます。
ContextはDBクライアントなど各種ライブラリを使う際に、対応する関数の引数にするだけでも動作します。
Contextはとても抽象度の高い存在ですが、実体はわずか数百行のコードで完結したライブラリです。
それだけの行数で動作するよう、非同期処理、インターフェースが高度に実装されています。
詳細な実装まで読み解いて、Contextをしっかりと理解してみたくなりませんか。

---

# Go Contextを完全に理解する

# 概要

Goではcontext.Contextを利用することで、キャンセルやタイムアウトを効率よく安全に実装することができます。

下記の３つのトピックで、Contextの概要から、詳細な仕組みまで、実際のcontext.Contextの実装を読み解きながら説明します。

## context.Contextとは

初心者の方でも理解できるよう、contextがどのような目的で使われるかを説明します。

## Contextの使い方

タイムアウト、キャンセル、任意の値のセット、取得といった方法を具体的に紹介します。

## Contextが動作する仕組み

context.Contextは抽象度の高さから想像できるイメージに反して、わずか数百行のコードで完結したライブラリです。

Contextの各種機能がどのように実装されているのか、コードリーディングして読み解いてみましょう。

# 対象

初心者〜上級者

# 言語

日本語(資料は英語にします)