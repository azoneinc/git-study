# Basic Commits

`git add` と `git commit` コマンドを紹介します。もし `git status`、`git log --oneline --graph`、`git add`、`git commit` を十分に使用している場合はおそらくスキップしても良いでしょう。
まだ基本的な Git の設定していない場合は、このファイルの下部を確認してください。

## セットアップ

1. `source setup.sh`（または PowerShell の場合は `.\setup.ps1`）を実行する

## 課題

1. `git status` を使用して、現在どのブランチにいるか確認する
2. `git log` はどのように表示されるか確認する
3. ファイルを作成する
4. 現在の `git status` の出力はどのようになっているか確認する
5. ファイルをステージングエリアに `add` する
6. 現在の `git status` はどのようになっているか確認する
7. ファイルをリポジトリに `commit` する
8. 現在の `git status` はどのようになっているか確認する
9. 先ほど作成したファイルの内容を変更する
10. 現在の `git status` はどのようになっているか確認する
11. 変更されたファイルを `add` する
12. 現在の `git status` はどのようになっているか確認する
13. 再度ファイルを変更する
14. `commit` を行う
15. 現在の `status`と`log` はどのようになっているか確認する
16. 最新の変更を add して commit する

## 利用コマンド

- `git add`
- `git commit`
- `git commit -m "My commit message"`
- `git log`
- `git log -n 5`
- `git log --oneline`
- `git log --oneline --graph`
- `touch filename` でファイルを作成（または PowerShell では `sc filename ''`）
- `echo content > file` でファイルの内容を上書き（または PowerShell では `sc filename 'content'`）
- `echo content >> file` でファイルに内容を追記（または PowerShell では `ac filename 'content'`）

## Git 初期設定

1. `git config --global user.name "John Doe"`
2. `git config --global user.email "johndoe@example.com"`

- vim が苦手な人
  - `git config --global core.editor nano`
  - `git config --global core.editor "code --wait"`

- Windows の場合
  - `git config --global core.editor notepad`
  - `git config --global core.editor "code --wait"`
