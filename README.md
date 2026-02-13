# かうたす（Cautas）ランディングページ

カウンセラー・コーチ向け業務管理アプリ「かうたす」の説明サイト（LP）です。

## 技術スタック

- 静的HTML/CSS/JS
- Tailwind CSS（CDN）
- Cloudflare Pages

## ディレクトリ構造

```
cautas-lp/
├── index.html          # メインページ
├── assets/
│   └── images/         # 画像ファイル
└── README.md           # このファイル
```

## ローカルでの確認

ブラウザで `index.html` を直接開くか、ローカルサーバーを起動してください。

```bash
# Python 3の場合
python -m http.server 8000

# Node.jsの場合
npx serve .
```

## デプロイ（Cloudflare Pages）

```bash
npm init -y
npx wrangler pages deploy . --project-name=cautas-lp
```

## アプリURL

https://cautas.pages.dev
