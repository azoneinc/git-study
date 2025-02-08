# Advanced interactive rebase

新機能 Hello World を実装した。この機能はドキュメントと単体テストの両方が用意された状態になっているが問題点がいくつかある。履歴は未完成の状態のコミットが多く含まれており本来含まれるべきではないコミットが混ざっている。

履歴が複雑にならないよう `git rebase --interactive` を使用して履歴を修正する。幸運なことに機能開始直前のリリースタグ `v0.0` が存在する。この課題は単一の操作やコマンドの実行という明確な回答があるわけではないので各自で理解しやすいログを想定して回答する必要がある。

## Setup

1. Run `source setup.sh`（PowerShell の場合は `.\setup.ps1`）

## Task

1. ログを調査し何が起こったのか把握する
2. `git rebase --interactive v0.0` を使用して機能開発全体のログを編集する
3. rebase の機能を用いて履歴を整理し実際に意味をなすようにする
   1. `reword` - コメントの編集
   2. `squash` or `fixup` - コミットの統合
   3. `drop` - コミットの削除
   4. `edit` - コミット内容の編集
4. 　全体を一度に書き換えるかいくつかの変更を適用して再度 `git rebase --interactive v0.0` を実行して繰り返し整理するかは自由に判断してよい

### useful commands

- `ls -l`
- `tail -n +1 *`
  - 現在のディレクトリ内の全てのファイルの先頭から最後までの内容を出力する
- `git log --oneline`
- `git log --stat`
- `git log --patch`
- `git rebase -i <ref>`
