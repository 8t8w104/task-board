# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## GitHub リポジトリ

- URL: https://github.com/8t8w104/task-board.git
- メインブランチ: `main`

## Git 運用ルール

### コード変更後は必ず feature ブランチ経由で PR を作成する

main ブランチへの直接プッシュは禁止。必ず以下の手順で行うこと：

1. main を最新化してから feature ブランチを作成する
   ```
   git checkout main
   git pull origin main
   git checkout -b feature/作業内容
   ```

2. 変更内容を確認してステージングする
   ```
   git status
   git diff
   git add <変更したファイル>
   ```

3. コミットする（何を変更したか分かるメッセージで）
   ```
   git commit -m "コミットメッセージ"
   ```

4. feature ブランチをプッシュする
   ```
   git push origin feature/作業内容
   ```

5. Pull Request を作成する
   ```
   gh pr create --title "タイトル" --body "変更内容の説明"
   ```

6. PR をマージして main に取り込む
   ```
   gh pr merge --merge --delete-branch
   ```

- コード変更のたびに必ずプッシュすること（作業終了時のまとめプッシュは不可）
- PR の作成からマージまで GitHub CLI (`gh`) を使って完全自動で行うこと
- マージ後はリモートの feature ブランチを削除すること（`--delete-branch`）
