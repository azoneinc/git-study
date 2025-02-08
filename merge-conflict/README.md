# Merge Conflict

## セットアップ

1 Run `source setup.sh`（PowerShell の場合は `.\setup.ps1`）

## 課題

`merge-conflict-branch1` で追加された内容と `master` の内容がコンフリクトしているため手動でのマージが必要。完了時には両方の変更が `master` に含まれている必要がある。

1. `git merge` を使用して `merge-conflict-branch1` の変更を master に取り込む
2. 現在の `git status` の内容を確認する
3. 任意のエディタでコンフリクトを解消する
4. `git status` で表示される内容を確認し内容に従ってマージを完了する
5. `git log --oneline --graph` の内容を確認する

## 利用コマンド

- `git merge`
- `git status`
- `git add`
- `git commit`
- `git log --oneline --graph`
