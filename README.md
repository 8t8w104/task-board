# task-board

タスク管理アプリケーションです。

## Claude Code での開発について

このリポジトリは Claude Code を使って開発を進めています。

### 事前準備

GitHub CLI をインストールし、以下のコマンドで認証しておくことで、Claude がコミット・プッシュから Pull Request の作成まで一貫して行えます。

```bash
gh auth login
```

認証後は Claude に「変更してプッシュして PR を作って」と指示するだけで、ブランチ作成からプルリクエスト作成まで自動で対応します。