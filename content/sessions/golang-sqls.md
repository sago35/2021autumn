---
key: golang-sqls
title: Golangで作るSQL Language Server(sqls)
id: golang-sqls
format: conference
talkType: ""
allroom: false
speakers:
- lighttiger2505
---
私はGo言語でsqlsというSQL Language Serverを作りました。sqlsはSQLを静的解析し、DBから取得されたテーブルやカラム情報を組み合わせて、自動補完やドキュメント表示など、開発に必要なインテリセンスを提供するサーバーです。
利用するクライアントとの通信にLanguage Server Protocol(LSP)を用いることであらゆるエディタが、sqlsの支援を受けることができます。

---

今回、私が語りたいのはsqlsの機能や、ユーザーがsqlsを利用して得られるメリットではなく、その製造プロセスです。
自分がカスタマイズしたエディタでSQLの自動補完を動かしたい。その熱意だけで、構文解析の手法を何一つ知らなかった私は多くの不明瞭な事柄に立ち向かいました。

- LSPの仕様とGo言語でのjson-rpc2サーバーの実装方法
- 自動補完のためのnon-validation parserとその実装方法
- 複数のデータベースへの対応
- 継続的開発のためのテストの整備

普段何気なく利用して私たちの開発体験を良くしてくれるツールですが、
創意工夫をすることで、自分でもこれを作ることもでき、充実した時間を得られるということを伝えたいと思います。
また、今回Go言語採用してsqlsを製造したことで、気づいたGo言語の利点などについても話します。