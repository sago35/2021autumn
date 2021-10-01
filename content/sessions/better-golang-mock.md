---
key: better-golang-mock
title: golang/mockでのモック生成と管理の "より良い" アプローチ
id: better-golang-mock
format: conference
talkType: ""
allroom: false
speakers:
- sanpo_shiho
---
golang/mockというinterface定義からモックを生成するGoのツールがあります。
このLTではgolang/mockの生成と管理に特化したgomockhandlerというツールの紹介をします。
https://github.com/sanposhiho/gomockhandler

---

コード生成を行うツールを導入する際、多くの場合で「(1)どのように生成するか」とその後「(2)生成したコードをどのように管理するか」の少なくとも二つの考慮点が増えることとなります。

1に関してはGoではgo generateが使用されることが多く、また、2に関してはGitHubで通常のコードと同時に管理されるのみとなる場合が多いです。
しかし、ツールによってはgo generateでコードを生成することが最適ではなかったり、「更新(= コードの生成し直し)忘れ」を防止する仕組みが必要となる場合があります。そして、一つ一つ順番にモックを生成する必要がなく、また、対象のinterfaceの更新のたびにモックを生成し直す必要があるgolang/mockはこの二つの点に当てはまります。
このLTでは gomockhandler というこれらの改善点を背景としたツールの紹介と、gomockhandler ではどのようにこれらの問題を解決しているかという内容の話をします。