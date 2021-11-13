---
key: fast-scalable-reverse-geocoding
title: Goで超高速かつスケーラブルな逆ジオコーディングAPIサーバーを作ってみた
id: fast-scalable-reverse-geocoding
format: conference
talkType: ""
allroom: false
speakers:
- erakazu
videoId: w2m4u3wruJY?start=5942
---
モビリティサービスでは緯度経度を住所に変換しなければならない場面が多々あります。SaaS APIでこの機能が提供されていますが、それらでは望む変換結果を得られない場面もあり、また、費用もそれなりにかかります。
そこで、外部SaaSに頼らずGolangを使って逆ジオコーディングAPIを自作することにしました。C言語で実装されたライブラリをCGO経由で活用しつつ、Go側の実装やデータの最適化を行うことで、usecオーダーで変換処理が完了する超高速なサービスを実現しました（APIの性能としてはHTTPのオーバーヘッドが支配的なレベルです）。
本セッションでは実装上工夫した点などを紹介します。
