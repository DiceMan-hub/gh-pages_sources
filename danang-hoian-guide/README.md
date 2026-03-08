# ダナン＆ホイアン 家族観光ガイド 2026（公開用）

このフォルダは **`gh-pages_sources` リポジトリ** のコンテンツのひとつです。  
リポジトリ名は用途（Pages 用ソース置き場）、コンテンツ名（vietnam-family-guide など）はこのサブフォルダで区別します。

## リポジトリ名

- **リポジトリ**: `gh-pages_sources` … Pages 用ソースをまとめる汎用名
- **このコンテンツ**: サブフォルダ `danang-hoian-guide` … 内容ごとのパス

公開後の URL:  
`https://<ユーザー名>.github.io/gh-pages_sources/danang-hoian-guide/`

## 公開の手順

### 1. GitHub で新しいリポジトリを作成

- https://github.com/new を開く
- **Repository name**: `gh-pages_sources`
- **Public** を選択
- **Add a README file** は不要
- Create repository

### 2. リポジトリのルート（gh-pages_sources）で Git 初期化して push

※ 実行するのは **Vault 内の `gh-pages_sources` フォルダ**（このフォルダのひとつ上）です。

```bash
cd "gh-pages_sources"
git init
git add README.md danang-hoian-guide/
git commit -m "Add danang-hoian-guide: ダナン&ホイアン 家族観光ガイド 2026"
git branch -M main
git remote add origin https://github.com/<あなたのユーザー名>/gh-pages_sources.git
git push -u origin main
```

※ 今後ほかのガイドを追加するときも、同じリポジトリに別サブフォルダ（例: `other-guide/`）を add して push すれば、`.../other-guide/` で公開できます。

### 3. GitHub Pages を有効化

- リポジトリの **Settings** → **Pages**
- **Source**: Deploy from a branch
- **Branch**: `main` / `/ (root)` を選択
- Save

数分後に次の URL で表示されます：

`https://<あなたのユーザー名>.github.io/gh-pages_sources/danang-hoian-guide/`

---

- **Hero 画像**: `danang_hoian_header.png` をこのフォルダ（`danang-hoian-guide`）に置くと表示されます。なければグラデーションで表示されます。
- 元の Obsidian 用 HTML: `01_OurStory/Vietnam/ダナン&ホイアン_家族観光おすすめガイド_2026.html`
