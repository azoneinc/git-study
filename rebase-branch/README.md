# rebase branch

## セットアップ

1. `source setup.sh` を実行する（または PowerShell では `.\setup.ps1` を実行する）

## 課題

1. 存在するブランチを確認する
2. master ブランチのログを確認する
3. uppercase ブランチに切り替える
4. ログが master ブランチのログとどのように異なるか確認する
5. uppercase ブランチを master でリベースする (`git rebase master`)
6. uppercase ブランチのログを確認する
7. 次に master ブランチに切り替える
8. uppercase ブランチを master ブランチにマージする
9. 現在のログがどのようになっているか確認する

## 便利なコマンド

- `git switch <branch-name>`
- `git rebase <branch-name>`
- `git log --oneline --graph --all`
- `git merge <branch-name>`
