---
key: gorm-update
title: Gormのバージョンを上げたお話
id: gorm-update
format: conference
talkType: ""
allroom: false
speakers:
- sntree_suzunoki
---
RettyではGo製のマイクロサービスでGORMを採用していますが、Version2リリースではいろいろなつまづきがあり苦労しました。
バージョンアップの過程での大変だったことや学んだことを共有します。

---

- Gormについて
    - 簡単な紹介
    - v2アップデートの概要
- v2アップデートで行ったこと
    - 破壊的変更への対応
    - Rettyでの使われ方について
- 大変だったこと、ハマったこと、学んだこと
    - 圧倒的物量
    - タグの使い方
    - パフォーマンスを出すために
- これから取り組む方へのアドバイス