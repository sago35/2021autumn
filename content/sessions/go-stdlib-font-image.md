---
key: go-stdlib-font-image
title: Goの標準ライブラリで扱うフォントと画像
id: go-stdlib-font-image
format: conference
talkType: ""
allroom: false
speakers:
- _achiku
---
Goは一見不思議に思えるけどとても実践的なInterfaceを提供していると、私は考えています。`net/http` はその一例です。APIサーバーを書くソフトウェアエンジニアとして `net/http` には馴染みがあるのですが、ちょとした興味から触った `image/draw` や `golang.org/x/image/font` にも同じように一見不思議に見えるが実践的なInterfaceがあるなと感じました。その内容を、これらのパッケージを初めて見る方たちにも分かりやすいように実例を用いて説明します。最後には、Goの画像処理に興味を持った理由である自作Webサービスも紹介します。

---

- image
    * `image` と `image/draw` パッケージを利用した基礎的な画像操作 
        * ource-over-destination と sourceという操作の説明
        * src/dst/mapという3つの概念と画像内位置情報をを利用することで、基礎的な画像操作を行う例を示す
- font
    * 基礎的な概念の説明
        * Font
            * 「フォントとは正確にはグリフ集合とよばれる特定の文字セットと、特定の書体デザインにもとづく文字のかたちの集合である」
        * TrueType/OpenType
            * フォント配布形式
            * TrueTypeの上位互換であるOpenTypeという形式も存在する
            * OpenTypeは「合字」「異体字の制御」「柔軟な文字詰め」等ができる
            * Goは標準ライブラリを利用してTrueTypeとOpenType両方扱えるようになっている
        * Font File
            * フォントファイフ形式にのっとって作成されたファイル
        * Glyph
            * フォントの中の文字(字形)をグリフ(glyph)と呼ぶ
            * 印刷やコンピュータ上で用いられる書体を、通常フォントと呼び、個々の字形をグリフ(Glyph)と呼ぶ
    * Glyphを描画する
        * imageの章で説明したsrc/dst/mapという3つの概念を利用し、1つGlyphを描画する
            * 例示する
        * imageの章で説明したsrc/dst/mapという3つの概念を利用し、複数のGlyphを描画する
            * 概念
                * https://developer.apple.com/library/archive/documentation/TextFonts/Conceptual/CocoaTextArchitecture/Art/glyph_metrics_2x.png
                * 重要な概念はadvancementとkern
            * `x/image/font` 内部の `Drawer.DrawString` の処理を説明する
                * この中でimageの章で説明したsrc/dst/mapがどのように応用されているかを説明
        * 文字を特定の幅で折り返すために何が必要か
            * 先行ライブラリを探す
                * https://github.com/fogleman/gg
                    * https://github.com/fogleman/gg#text-functions
                    * 内部はスペースで単語が区切られるものを前提に作られており、日本語では機能しない
            * 日本語を前提とした折返しとAlignの実装として考えられる形
- 何に使うのか
    * SNS上で特定画像に自身が入力した文字を埋め込み、OGPを主体としてコミュニケーションできるWebサービス
    * (これは当日までにサーバーを公開できるようにします)
