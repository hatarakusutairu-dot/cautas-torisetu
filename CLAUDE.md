# CLAUDE.md - かうたす（Cautas）LP

## プロジェクト概要
カウンセラー・コーチ向け業務管理アプリ「かうたす」のランディングページ（LP）

## 技術スタック
- 静的HTML/CSS/JS（フレームワーク不使用）
- Tailwind CSS（CDN経由）
- デプロイ先: Cloudflare Pages

## ディレクトリ構造
```
cautas-lp/
├── index.html          # メインLP（単一ファイル）
├── assets/
│   └── images/         # スクリーンショット等の画像
├── README.md
└── CLAUDE.md
```

## デザイン方針
- カラー: 緑系（primary: #10b981, dark: #059669）
- UI: 丸みのある優しいデザイン（border-radius多用）
- エフェクト: ガラスモーフィズム（backdrop-filter: blur）
- レスポンシブ: モバイルファースト

## LPセクション構成
1. ヒーロー（キャッチコピー + CTA）
2. 課題提起（カウンセラーの悩み3つ）
3. 機能紹介（8機能）
4. 特徴・強み（AI、シンプルUI、データ一元管理）
5. 料金プラン（現在無料）
6. FAQ（5問）
7. CTA + フッター

## 重要なリンク
- アプリ本体: https://cautas.pages.dev
- LP: https://cautas-lp.pages.dev（デプロイ後）

## デプロイコマンド
```bash
npx wrangler pages deploy . --project-name=cautas-lp
```

## 編集時の注意
- Tailwind CDNを使用しているため、ビルド不要
- カスタムCSSは`<style>`タグ内に記述
- アイコンはSVGをインライン記述（外部依存なし）
