# Basic Staging

git のステージングエリアを検証する。git では 3 つの異なる領域で作業する。

* 変更している作業ディレクトリ
* git add で追加したすべての変更が残るステージングエリア
* すべてのコミットが蓄積され履歴となるリポジトリ
  * ステージングされた変更をここに反映するには git commit コマンドを実行する

ファイルは作業ディレクトリとステージングエリアの両方で差分を持つことができる。これらの差分が同一である必要はない。

ファイルのステージングされた変更を復元するために git restore を使用し、ファイルを以前の状態に戻すため git checkout を使用する。

## セットアップ

1 Run `source setup.sh`（PowerShell の場合は `.\setup.ps1`）

## 課題

リポジトリで作業している　`file.txt` というファイルが存在する。

1. file.txt の内容は何か
2. file.txt の内容を上書きして作業ディレクトリ上の状態を変更する　`echo 2 > file.txt`（PowerShell の場合は `sc file.txt '2'`）
3. git diff は何を示しているか
4. git diff --staged は何を示しているか　なぜこれが空なのか
5. 作業ディレクトリから変更をステージするために git add file.txt を実行する
6. git diff は何を示しているか
7. git diff --staged は何を示しているか
8. file.txt の内容を上書きして作業ディレクトリ上の状態を変更する　`echo 3 > file.txt`（PowerShell の場合は `sc file.txt '3'`）
9. git diff は何を示しているか
10. git diff --staged は何を示しているか
11. 何が起こっているか説明する
12. git status を実行し　出力に file.txt が 2 回表示されることを確認する
13. 変更のステージを解除するために git restore --staged file.txt を実行する
14. 現在の git status は何を示しているか
15. 変更をステージし commit を作成する
16. ログはどのように表示されるか
17. file.txt の内容を上書きする　`echo 4 > file.txt`（PowerShell の場合は `sc file.txt '4'`）
18. file.txt の内容は何か
19. git status は何を示しているか
20. git restore file.txt を実行する
21. file.txt の内容は何か
22. git status は何を示しているか

## 利用コマンド

* `git add`
* `git commit`
* `git commit -m "My lazy short commit message"`
* `git log`
* `git log -n 5`
* `git log --oneline`
* `git log --oneline --graph`
* `git restore --staged`

## Aliases

以下のようにエイリアスを設定できる。

`git config --global alias.lol 'log --oneline --graph --all'`
