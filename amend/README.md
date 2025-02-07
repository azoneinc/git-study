# Amending commits

`git commit --amend` を使うと直前のコミットを修正できます。
`git log -p` や `git show` を使って直前のコミットの内容を確認して必要な修正を加えましょう。

## セットアップ

1. `source setup.sh`（または PowerShell の場合は `.\setup.ps1`）を実行する

## 課題

1. `git status` の内容を確認する
2. `git log -p` の内容を確認する
3. bar.txt の変更をステージする
4. `git commit --amend` を実行する
5. `git log -p` の内容を確認する
6. もう一度 `git commit --amend` を実行するとどうなるか確認する

## 便利なコマンド

- `git add`
- `git log --oneline --graph`
- `git log -p`
- `git show`
- `git commit --amend`
