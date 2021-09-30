---
key: go-proposal-guide
title: GoのProposalの追い方ガイド
id: go-proposal-guide
format: conference
talkType: ""
allroom: false
speakers:
- __syumai
---
Go projectにおいて、何か言語、ライブラリ、ツールへの重要な変更が行われる場合は、これに対して議論を行うためのデザインが必要となります。
この時、変更の提案元がGo Teamであろうと、外部からであろうと、同じプロセスを経ます。
このプロセスの初めに提出されるのが、Proposalです。

将来のGoがどうなっていくのか、短期的、長期的にキャッチアップをし続けたいのであれば、Proposalをウォッチするのは非常に有効な手段となります。
本発表では、ここ最近、Generics関連の動向を追いかけていく中で知ったProposalの追い方について、知っておくべき点をまとめて説明します。

---

Goの最新動向を追うにあたって、Proposalへのキャッチアップは欠かせません。
Proposalは、誰でも簡単にGitHub Issueの形式でGo projectに対して提出することが出来ます。
その分、ウォッチするにあたっては、重要なProposalがどれかをある程度見分ける必要が出て来ます。

先日、Go 1.17 リリースパーティーにてGenerics関連のProposalの動向をまとめて以来、アップデートを追い続けているので、その経験の中から得られたProposalの追い方について説明します。

---

* GitHub Projectを使ったProposalのステージの運用
* GitHub Issue / Discussion上で行われる議論内容の見方
* 『Proposing Changes to Go』に記載の重要事項

などについて説明を行います。