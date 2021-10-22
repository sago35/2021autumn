---
key: go-unicode
title: "「\U0001FAA6問題」から考えるGoのUnicodeサポート"
id: go-unicode
format: conference
talkType: ""
allroom: false
speakers:
- ymtyta
---
SpannerとGoでサービス開発をしたときに、「🪦問題」に遭遇しました。
🪦が\U0001faa6になってしまった事象に遭遇したところから、Unicodeのリリースサイクルと、Goの追随状況、Unicodeサポート方法、spanner.NullStringを通してfmt.Sprintfの実装方法を調べました。
本セッションでは、調査した知見を共有することで、GoのUnicodeサポートについて少し詳しくなり、spanner.NullStringやfmt.SprintfとUnicodeのハマりどころを知ってもらえるセッションをお届けします。