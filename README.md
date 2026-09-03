# 日本経済モニター(公開ダッシュボード)

このリポジトリは **Public** — GitHub Pagesとして公開するための静的サイトのみを置く。

- `index.html` … ダッシュボード本体(データ取得ロジックは含まない)
- `data/latest.json` … 表示用データ。**手で編集しない** — 別リポジトリ
  ([japan-economy-fetcher](https://github.com/))の GitHub Actions が
  毎日自動でこのファイルを書き換えてpushする。

セットアップ手順は `japan-economy-fetcher/README.md` を参照。
