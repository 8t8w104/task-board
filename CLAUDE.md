# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## GitHub リポジトリ

- URL: https://github.com/8t8w104/task-board.git
- メインブランチ: `main`

## Git 運用ルール

### コード変更後は必ず GitHub にプッシュする

コードを変更するたびに、以下の手順で GitHub にプッシュすること：

1. 変更内容を確認する

   ```
   git status
   git diff
   ```

2. 変更ファイルをステージングする

   ```
   git add <変更したファイル>
   ```

3. コミットメッセージは変更内容を端的に表す日本語または英語で記述する

   ```
   git commit -m "コミットメッセージ"
   ```

4. GitHub にプッシュする
   ```
   git push origin <ブランチ名>
   ```

- コード変更のたびに必ずプッシュすること（作業終了時のまとめプッシュは不可）
- コミットメッセージは何を変更したかが分かるように具体的に書くこと
- main ブランチへの直接プッシュは避け、feature ブランチを使うこと
