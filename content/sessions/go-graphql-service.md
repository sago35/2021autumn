---
key: go-graphql-service
title: GoとGraphQLを使用したサービス開発
id: go-graphql-service
format: conference
talkType: ""
allroom: false
speakers:
- flum_
---
Rettyの新規事業Retty OrderはバックエンドにGoとGraphQLを採用し開発を行っています。
新規事業は刻々と状況が変わっていきます。ただ機能を開発するだけではなく、品質と速度の両立や今後の運用やスケールを見据えた開発を行っていく必要があります。
開発で工夫している点や採用技術など、どのように開発行っているのかご紹介します。

---

- Goの採用理由
- Clean Architecture
- GraphQLでスキーマ駆動開発
  - 99designs/gqlgenの知見
    - Redisを使用したSubscriptionの実装
- テスト観点
  - それぞれのレイヤーでのテスト観点
- 工夫していること
  - Code generate(go-task)
  - レプリカラグ
    - ローカルでは必ず1秒のレプリカラグを発生させている
  - データベースモデルの自動生成
  - Redisの負荷を減らす仕組み
    - アプリケーション内部のPub/Sub