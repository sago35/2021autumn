---
key: handmade-http-router
title: net/httpでつくるHTTPルーター自作入門
id: handmade-http-router
format: conference
talkType: ""
allroom: false
speakers:
- bmf_san
---
Goの標準パッケージであるnet/httpを使ってHTTPルーターを自作する方法についてお話します。

net/httpを使った簡単なサーバーを起動するコードの読み解きから始めて、HTTPルーターの自作方法、アルゴリズムについて解説します。

優秀なルーターがOSSとして存在しているため、あまり自作するような機会はないかもしれませんが、自作を通して、net/httpや木構造への理解を深めることができます。

本LTはGoの入門者をターゲットとして、Goの理解につながるきっかけとなるような話になればと思っています。

---

[goblin](https://github.com/bmf-san/goblin)という自作のHTTPルーターを作っています。

このルーターは、Goの標準パッケージだけで構成されており、net/httpのインターフェースとの互換性を保つように実装されています。

ルーターの自作を通して、私が学び得た知見についていくつかのブログ記事とスライドにまとめています。

- [GolangのHTTPサーバーのコードリーディング](https://bmf-tech.com/posts/Golang%E3%81%AEHTTP%E3%82%B5%E3%83%BC%E3%83%90%E3%83%BC%E3%81%AE%E3%82%B3%E3%83%BC%E3%83%89%E3%83%AA%E3%83%BC%E3%83%87%E3%82%A3%E3%83%B3%E3%82%B0)
- [URLルーティング自作入門　エピソード１](https://bmf-tech.com/posts/URL%E3%83%AB%E3%83%BC%E3%83%86%E3%82%A3%E3%83%B3%E3%82%B0%E8%87%AA%E4%BD%9C%E5%85%A5%E9%96%80%E3%80%80%E3%82%A8%E3%83%94%E3%82%BD%E3%83%BC%E3%83%89%EF%BC%91)
- [URLルーティング自作入門　エピソード２](https://bmf-tech.com/posts/URL%E3%83%AB%E3%83%BC%E3%83%86%E3%82%A3%E3%83%B3%E3%82%B0%E8%87%AA%E4%BD%9C%E5%85%A5%E9%96%80%E3%80%80%E3%82%A8%E3%83%94%E3%82%BD%E3%83%BC%E3%83%89%EF%BC%92)
- [Introduction to URL router from scratch with Golang](https://dev.to/bmf_san/introduction-to-url-router-from-scratch-with-golang-3p8j)
- [GolangでURLルーターをつくった](https://speakerdeck.com/bmf_san/golangteurlrutawotukututa)

本LTはこれらの内容を10分に総括したものとなります。