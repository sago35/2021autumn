---
key: webdriver-client-from-scratch
title: Create Go WebDriver Client from Scratch
id: webdriver-client-from-scratch
format: conference
talkType: ""
allroom: false
speakers:
- hgsgtk
---
Webアプリ開発をしている現場ではUIレベルのブラウザ操作を自動化することによって実現する自動テストの作成は馴染みが深いものです。

ブラウザ操作の自動化にあたり出てくる WebDriver の Client はその仕様上 net/http パッケージ等の標準パッケージを介して自作することができます。

本トークでは、W3C勧告の標準化仕様WebDriver Wire Protocol等の詳細に軽く触れた上で、net/httpパッケージ等標準パッケージを組み合わせることでWebDriverとコミュニケーションをしブラウザを動かす実装方法を解説します。

---

聴講者的な目線での期待設定としては、「WebDriverの仕様を理解して明日に活かす」と言うよりかは、「Goで実装するアイデアのバリエーションを増やす刺激になる」という後者を意識しています。

Goの特筆した点の一つは標準パッケージの機能性、それらの組み合わせてthird party packageを必須としなくても、自分のアイデアを実現できる点にあると考えます。WebDriverについてご存じの方であれば自明な話になるのですが、基本的にWebDriverはclient-serverの関係性でJSON HTTP APIがI/Fとなっています。ゆえに、本トークで紹介予定のWeb Driver clientについても多少のthird party packageを用いるかもしれませんが、主たる機能性については標準パッケージにて実装することになると想定しています。

多少WebDriverについての雑学を知りつつ、「このくらいブレークダウンすれば確かにGoで実装できるなぁ」的な"刺激"を、カンファレンスの締めの場になるLTにひと添えできればと思っております。