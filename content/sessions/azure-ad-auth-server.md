---
key: azure-ad-auth-server
title: (仮) Azure ADに完全対応した認証プロキシ・webサーバを開発してみた話
id: azure-ad-auth-server
format: conference
talkType: ""
allroom: false
speakers:
- hogegashi
---
AzureにはApp ServiceやStatic Web Appsといったwebサイト構築に便利なPaaSがあり、Easy Authという組み込みの認証・認可機能を備えています。しかしながらエンタープライズ水準のきめ細かなアクセス制御が必要な場合は、開発者は依然として自分でその機能をwebアプリ中に組み込む必要がありました。今回、企業内webサイトのような、細かなアクセス制御の要件はあるがwebアプリにするまでもない静的webサイトを誰でも簡単に構築できることを目標として、Azure ADに対応した認証プロキシ・webサーバをGo言語で実装しましたので、実際の構築手順や事例と共に紹介します。