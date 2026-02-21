# Niigata Private Guide Site (Astro)

新潟県限定の通訳案内士向け集客サイトです。  
Astroで構築した静的サイトなので、表示速度を重視した構成です。

## 1. 開発環境

- Node.js 20 以上（推奨: 22 LTS）
- npm

## 2. ローカル起動

```bash
npm install
npm run dev
```

ブラウザで `http://localhost:4321` を開いて確認できます。

## 3. 本番ビルド

```bash
npm run build
```

`dist/` に静的ファイルが出力されます。

## 4. GitHub 登録手順

```bash
git add .
git commit -m "Create Niigata guide marketing site with Astro"
git branch -M main
git remote add origin <YOUR_GITHUB_REPO_URL>
git push -u origin main
```

## 5. Cloudflare Pages デプロイ

1. Cloudflare Dashboard -> `Workers & Pages` -> `Create application` -> `Pages` を選択  
2. GitHubリポジトリを接続  
3. Build settings を以下で設定

- Framework preset: `Astro`
- Build command: `npm run build`
- Build output directory: `dist`
- Node version: `22`

4. `Save and Deploy` で公開

## 6. サイト内容

- 新潟県限定・欧米系ターゲット向け
- 3つのモデルルート（料金・所要時間・集合場所・歩行レベル・見どころ）
- 料金に含む/含まない項目
- キャンセル規定、支払い方法、問い合わせ導線
- 年配の方でも見やすい大きめ文字とシンプルUI
