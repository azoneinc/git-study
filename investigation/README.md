# Git objects

Objects は `<repository>/.git/objects` 内に保存される　sha の最初の 2 文字と一致するサブフォルダ内に配置される。`fc1da6e8f` はファイル `.git/objects/fc/1da6e8f` を指している。

`git ls-tree master .` はフォルダの内容を展開して一覧表示す。

`git cat-file` は渡された _ref_ の内容を展開し表示する。通常はオブジェクトのハッシュとオブジェクトのタイプを指定する必要があるが `-p` オプションはオブジェクトのタイプを自動で判別し内容を整形して表示する。

## セットアップ

1 Run `source setup.sh`（PowerShell の場合は `.\setup.ps1`）

## タスク

1. git ls-tree と git cat-file を使用して Git のデータ構造を見る

- どの tree および blob オブジェクトが存在しそれらは何を指しているか
- どのコミットがこのグラフ内のどこを指しているか
