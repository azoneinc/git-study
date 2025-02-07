# Reordering history

## セットアップ

1. `source setup.sh`（または PowerShell の場合は `.\setup.ps1`）を実行する

## 課題

 `git log` でログを確認するとファイル名に対してコミット順序が無茶苦茶になってしまっている。
`rebase`コマンドを用いてファイル名に沿った順番でコミットログを整理する。

1. `git log --oneline --graph` を使用してログを確認する
2. `git rebase -i <after-this-commit>` を使用してコミットの順序を変更する
   1. 編集画面で使用可能なコマンドの説明がコメントとして記載されているので確認する
3. `git log --oneline --graph` を使用して結果を確認する

### 便利なコマンド

- `git rebase -i <after-this-commit>`
- `git log --oneline --graph`
- `git reflog`
