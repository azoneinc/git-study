# Detached head state

ユーザーが "detached head" 状態になると恐ろしい状況に見えるが Git は恐ろしくない

## セットアップ

1. Run `source setup.sh`（PowerShell の場合は `.\setup.ps1`）

## タスク

1. `git status` と `git log --oneline --graph --all` を実行して状況を確認する
2. `master` に移動してこのリポジトリの通常状態を回復する

※ ターミナルで `setup.sh` を実行していない場合、このタスクはより混乱するかもしれない。

最初のコミットのメッセージが `A` であるものから作成された `the-beginning` というブランチを作成したい。

3. まず detached head 状態を発生させることでこれを実現できるか

## 便利なコマンド

- `git status`
- `git log --oneline --graph --all`
- `git checkout <ref>` または `git switch --detach <ref>`
