# Interactive rebase with --autosquash option

新機能 Hello World を実装した。この機能はドキュメントと単体テストの両方が用意されているがドキュメントにタイプミスがある。これを修正し美しい履歴を得るために `rebase` する必要がある。

幸運なことに機能開始直前のリリースタグ `v0.0` が存在する。`git commit` と `git rebase` のオプションを使用すれば簡単に修正する方法がある。

## Setup

1 Run `. setup.sh`（PowerShell の場合は `.\setup.ps1`）

## Task

1. リポジトリと履歴を調査しドキュメントファイルが追加されたタイミングを把握する
2. `README.md` を修正しステージングする
3. 修正するコミットの sha を指定して `git commit --fixup=<commit id to be fixed>` でコミットする
4. `git rebase --autosquash --interactive v0.0` を使用して自動生成された rebase の編集画面を確認する
   1. `git commit --fixup` で追加されたコミットが指定したコミットに fixup されるようコミットの順番が自動で変更されている
5. `git log` を使用して履歴を確認する

### useful commands

- `ls -l`
- `tail -n +1 *`
- `git log --oneline`
- `git log --stat`
- `git log --patch`
- `git show <commit id>`
- `git add`
- `git commit --fixup=<commit id>`
- `git rebase -i <ref>`
