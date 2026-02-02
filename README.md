# daiko-calendar-theme

## 開発環境

### 1 バージョン管理（GitHubセオリー）
- **公式連携**: ShopifyストアとGitHubリポジトリを直接接続。
- **除外設定**: `.gitignore` を用い、PC固有の `.shopify/` フォルダを管理対象から除外。
- **ブランチ運用**: 
  - `main`: 本番稼働中のテーマ。
  - `dev`: 開発・テスト用。

### 2 開発スタック
- **テンプレート**: Liquid (Shopify Dawn)
- **スクリプト**: Vanilla JS (依存関係なしのネイティブJavaScript)
- **スタイル**: インラインCSS / Dawn standard CSS

### 3 開発環境の構築
以下の手順に沿って構築を進めてください。
1. npm install -g @shopify/cli @shopify/theme
2. shopify auth login --store your-store-name.myshopify.com
3. shopify theme dev
