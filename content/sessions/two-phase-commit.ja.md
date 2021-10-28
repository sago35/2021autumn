---
key: two-phase-commit
title: 二相コミットなどの具体例に見るゴルーチンとチャネルの使いどころ
id: two-phase-commit
format: conference
talkType: ""
allroom: false
speakers:
- kojiaomatsu
---
実務で実際に遭遇したゴルーチンとチャネルの使用事例を通して、その一般的な使いどころを考えます。

CloudSQLとDatastore双方のデータの更新のためにGo言語で二相コミットの実装をした事例や、待ち時間がかかる処理をゴルーチンに逃がしAPI呼び出しのレイテンシを改善した事例を紹介します。
