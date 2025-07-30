# LINE to Sheets System

LINEからのメッセージを自動的にGoogleスプレッドシートに記録するシステムです。

## 機能

- LINEからのメッセージを受信
- ユーザー情報（ID、表示名）を取得
- タイムスタンプと共にGoogleスプレッドシートに自動記録

## 環境変数

以下の環境変数を設定してください：

- `LINE_CHANNEL_ACCESS_TOKEN`: LINEチャネルアクセストークン
- `LINE_CHANNEL_SECRET`: LINEチャネルシークレット
- `GOOGLE_SPREADSHEET_ID`: GoogleスプレッドシートのID
- `GOOGLE_SHEET_NAME`: シート名（デフォルト: Sheet1）
- `GOOGLE_CREDENTIALS_JSON`: GoogleサービスアカウントのJSONキー（文字列形式）

## デプロイ

Render.comでのデプロイに最適化されています。

1. GitHubリポジトリにコードをプッシュ
2. Render.comでWebサービスを作成
3. 環境変数を設定
4. 自動デプロイ

## エンドポイント

- `/`: システム状態確認
- `/health`: ヘルスチェック
- `/webhook`: LINE Webhook（POST）

