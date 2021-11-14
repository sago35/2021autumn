---
key: go-scheduling
title: スケジューラから学ぶGoランタイム 〜 code reading of runtime pkg〜
id: go-scheduling
format: conference
talkType: ""
allroom: false
speakers:
- saki_engineer
videoId: w2m4u3wruJY?start=14944
slides: https://speakerdeck.com/sakiengineer/sukeziyurakaraxue-bugorantaimu-code-reading-of-runtime-pkg
---
Goにおいて複数のゴールーチンを並行に実行するためのスケジューラは、Goランタイム内で実装されています。しかし現在のスケジューラの大枠が実装されたのは9年前のGo1.1であり、世の中におけるGoのスケジューラ解説はそのときに世に出た公式設計書を元に、視覚的な図ベースで組み立てられているものがほとんどです。本セッションでは、スケジューラの挙動について実際のruntimeパッケージ内のコードベースで理解することを目的に、スケジューラについての説明体系を再構築します。
