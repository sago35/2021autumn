---
key: webdriver-client-from-scratch
title: Create Go WebDriver Client from Scratch
id: webdriver-client-from-scratch
format: conference
talkType: ""
allroom: false
speakers:
- hgsgtk
videoId: EVUCSrj83uM?start=30117
slides: https://speakerdeck.com/hgsgtk/create-go-webdriver-client-from-scratch
---
Webアプリ開発をしている現場ではUIレベルのブラウザ操作を自動化することによって実現する自動テストの作成は馴染みが深いものです。

ブラウザ操作の自動化にあたり出てくる WebDriver の Client はその仕様上 net/http パッケージ等の標準パッケージを介して自作することができます。

本トークでは、W3C勧告の標準化仕様WebDriver Wire Protocol等の詳細に軽く触れた上で、net/httpパッケージ等標準パッケージを組み合わせることでWebDriverとコミュニケーションをしブラウザを動かす実装方法を解説します。