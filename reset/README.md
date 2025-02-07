# Git reset

`reset` を使って変更のステージングの解除等様々な操作が可能です。reset のオプションである soft、mixed、hard の三種類の違いを理解することが目標です。

## セットアップ

1. `source setup.sh` を実行する（または PowerShell では `.\setup.ps1` を実行する）

## 課題

1. ワーキングディレクトリの状態を確認する
2. ログとステージの状況を確認する
3. `git reset --soft HEAD~1` を実行してみる
4. ワーキングディレクトリ、ログ、ステージがどうなるか確認する
5. `git reset --mixed HEAD~1` を実行する
6. ワーキングディレクトリ、ログ、ステージがどうなるか確認する
7. `git reset --hard HEAD~1` を実行する
8. ワーキングディレクトリ、ログ、ステージがどうなるか確認する
9. 次に `git revert HEAD~1` を実行してみる
10. ワーキングディレクトリ、ログ、ステージがどうなるか確認する

## 便利なコマンド

- `git log --oneline`
- `git commit --amend`
- `git status`
- `git reset --soft`
- `git reset --mixed`
- `git reset --hard`
- `git revert`
