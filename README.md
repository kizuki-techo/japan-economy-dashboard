# 日本経済モニター(公開ダッシュボード)

このリポジトリは **Public** — GitHub Pagesとして公開するための静的サイトのみを置く。

- `index.html` … ダッシュボード本体(データ取得ロジックは含まない)
- `data/latest.json` … 表示用データ。**手で編集しない** — 別リポジトリ
  ([japan-economy-fetcher](https://github.com/))の GitHub Actions が
  毎日自動でこのファイルを書き換えてpushする。
- `data/commentary.json` … ダッシュボード下部の「解説」セクションの文章データ。
  こちらは自動更新ではなく **手動更新**。グラフの動きを見て内容を更新したい時は、
  Claudeに「ダッシュボードの解説を最新のグラフを踏まえて更新して」のように依頼し、
  このファイルを編集してpushする。フィールドは `readingPoints`(短期/中期/長期/国際収支
  それぞれの読み取りポイント)・`overall`(全体評価)・`plus`/`minus`(プラス面/マイナス面)・
  `outlook`(短期/中期/長期の見通し)・`updatedAt`(更新日、画面下部に表示)。

セットアップ手順は `japan-economy-fetcher/README.md` を参照。
