# Merge Mergesort

マージコンフリクトを解決する。以下の 2 つの異なるブランチが存在する。

* Mergesort-Impl
* master

マージコンフリクトを確認しファイルを適切に編集して解決する。

## セットアップ

1. `source setup.sh` を実行する（または PowerShell では `.\setup.ps1` を実行する）

## 課題

1. `git branch` を実行して存在する 2 つのブランチを確認する
2. `Mergesort-Impl` ブランチを `master` ブランチにマージする
   1. コンフリクトの発生によりマージが完了しないことを確認する
3. `git status`のメッセージに何をすべきか書いてあるので確認する
4. `git mergetool --tool=vimdiff` または任意のエディタでマージコンフリクトを解決しマージを完了する

## 関連コマンド

* `git branch`
* `git merge`
* `git status`
* `git mergetool --tool=vimdiff`
* `git add`
* `git commit`
