---
key: how-goroutine-works
title: goroutineの仕組みについて
id: how-goroutine-works
format: conference
talkType: ""
allroom: false
speakers:
- sivchari
videoId: EVUCSrj83uM?start=16039
slides: https://speakerdeck.com/sivchari/goroutinefalseshi-zu-minituite
---
私たちはgoというキーワードを用いることで、仕組みが分からずとも並行処理を容易に行うことができます。そこで、なぜGoではgoroutineにより効率的な並行処理を実現できているか説明します。
トークを通してgoroutineが既存のスレッドと異なりflyweightと呼ばれる理由を知ることができます。またgoroutineがどのように管理されているのかというスケジューラーの仕組みについても知ることができます。
そのため、ただgoroutineを使うというステップから、Goの言語的な仕組みを理解した上でgoroutineによる並行処理を用いることができるようになるでしょう。