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

---

* セッション形式
  * 20分のセッション
  * プレゼン資料と一部GolandでGoの実装コードやサンプルプログラムをデモします。
* 内容
  * GoのバージョンとUnicodeサポートによってテスト時に遭遇した🪦問題からUnicode/emojiとGoのサポート状況について詳細に調べました。
    * Unicodeは約1年に1回メジャーアップデートがされます。
    * それに合わせて、iOS/Androidも追随してアップデートで新しいemojiを追加しています。
    * Unicode/emojiのバージョンアップと、iOS/Androidがいつ追随しているのかを気にしたことがなかったのでいい機会なのでまとめました
    * iOS/Androidが対応すると、当然それらのemojiをバックエンドのGoで受信するようになります。
    * GoのUnicodeサポートの追随状況はどうなっているのでしょうか。
    * 追随できないとどういう問題があるのか、新しいGoバージョンを使う必要性が何故あるのかを見ます。
  * 今回はSpannerを使用していて遭遇したので、spanner.NullStringの関連部分を紹介します
  * fmt.SprintfでUnicode周りで問題が出る理由を見ていきます。
* アジェンダ
  * Introduction
  * 🪦問題とは
  * 🪦問題が発生する前提条件
  * Unicodeとemojiのバージョンについて
  * iOSとAndroidのemojiの追加追随状況
  * GolangのUnicodeサポートの追随状況
  * 🪦問題が発生した原因
  * spanner.NullStringで問題が発生する原因
  * fmt.Sprintfで問題が発生する原因
  * GolangのUnicodeサポートの実装方法（Unicodeパッケージを深掘りしてみよう）
  * 🪦問題を経て、リリースのために決断したこと
  * まとめ