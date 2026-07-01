# 和ごころ ── 日本の伝統医学を知る

漢方（漢方薬による治療・漢方診療）と鍼灸・あん摩マッサージなど、日本の伝統医学を一般の方にやさしく紹介する啓発サイトです。単一の `index.html` だけで動作します（外部ライブラリなし・レスポンシブ対応）。

## ファイル構成

- `index.html` … サイト本体（これ1つで完結）
- `README.md` … 本ファイル

## GitHub Pages での公開手順

### A. ブラウザだけで公開する（かんたん）

1. GitHub にログインし、右上の「＋」→ **New repository**。
2. リポジトリ名を入力（例：`kampo-site`）。**Public** を選び **Create repository**。
3. 作成後の画面で **uploading an existing file** をクリック。
4. `index.html` と `README.md` をドラッグ＆ドロップし、**Commit changes**。
5. リポジトリ上部の **Settings** → 左メニュー **Pages** を開く。
6. **Source** を **Deploy from a branch** にし、Branch を **main** ／ フォルダを **/ (root)** にして **Save**。
7. 1〜2分待つと、同じ Pages 画面に公開 URL が表示されます。
   （形式：`https://<ユーザー名>.github.io/kampo-site/`）

### B. コマンドラインで公開する

```bash
# このフォルダ（index.html がある場所）で実行
git init
git add index.html README.md
git commit -m "初回公開：和ごころ 日本の伝統医学サイト"
git branch -M main
git remote add origin https://github.com/<ユーザー名>/kampo-site.git
git push -u origin main
```

その後、**Settings → Pages** で Branch を `main` / `/ (root)` に設定して保存すれば公開されます。

## 更新のしかた

`index.html` を編集して再度アップロード（またはコミット＆プッシュ）すると、数分で公開ページに反映されます。

## 独自ドメインを使いたい場合

Settings → Pages の **Custom domain** にドメインを入力し、DNS 側で GitHub Pages 向けの設定（CNAME など）を行います。

## ご注意

本サイトは教育・啓発を目的としたものです。個々の症状の診断や治療は、必ず医師・薬剤師などの専門家にご相談ください。公開前に、掲載する数値・記述について専門家の監修を受けることをおすすめします。
