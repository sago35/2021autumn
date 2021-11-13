---
key: io-fs-testability
title: io/fsパッケージを用いたテスタブルなコード生成ツールの開発
id: io-fs-testability
format: conference
talkType: ""
allroom: false
speakers:
- tenntenn
videoId: EVUCSrj83uM?start=20833
---
io/fsパッケージによりOSのファイルシステムに依存しない処理を書けます。例えば、複数のファイルを生成するツールの開発において、生成したファイル群をtxtar形式で出力し、ファイルシステムとして扱うことでテストを容易にできます。また、複数のファイルにまたがるテンプレートをtxtar形式として扱い、それをファイルシステムとして解釈することでtext/templateパッケージでパースでき、保守しやすさと可読性を両立できます。本セッションでは、skeletonという静的解析ツールのコードの雛形を生成するツールの開発で用いているio/fsパッケージを使ったいくつかの手法についてご紹介します。