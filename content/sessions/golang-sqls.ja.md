---
key: golang-sqls
title: Golangで作るSQL Language Server(sqls)
id: golang-sqls
format: conference
talkType: ""
allroom: false
speakers:
- lighttiger2505
videoId: EVUCSrj83uM?start=18205
slides: https://speakerdeck.com/lighttiger2505/golangdezuo-rusql-language-server-sqls
---
私はGo言語でsqlsというSQL Language Serverを作りました。sqlsはSQLを静的解析し、DBから取得されたテーブルやカラム情報を組み合わせて、自動補完やドキュメント表示など、開発に必要なインテリセンスを提供するサーバーです。
利用するクライアントとの通信にLanguage Server Protocol(LSP)を用いることであらゆるエディタが、sqlsの支援を受けることができます。