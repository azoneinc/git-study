# Basic Ignore

`.gitignore` は追跡させたくないファイルの拡張子やフォルダ構造を指定できる。ちなみに `.gitignore` によって無視されたファイルやフォルダでも `git add -f` で強制的にステージすることは可能。

`git rm` はワーキングディレクトリからファイルを削除しその削除をステージする。
ファイルをリポジトリから削除する必要があるがワーキングディレクトリには残しておきたい場合、`git rm --cached` を使用してステージングエリアからのみ削除できる。

## セットアップ

1. `source setup.sh`（または PowerShell の場合は `.\setup.ps1`）を実行する

## 課題

1. `foo.s` という名前のファイルを作成する
2. `git status` の出力を確認する
3. ワーキングディレクトリに `*.s` を含む `.gitignore` ファイルを作成する
4. `git status` の出力を確認する
5. `.gitignore` ファイルをコミットする
6. `file1.txt` をコミットする
7. `.gitignore` ファイルに `*.txt` を含む行を追加して `txt` ファイルを無視対象にする
8. `git status` の出力を確認する
9. `file1.txt` を変更する
10. `git status` の出力を確認する
    1. `.gitignore` に `*.txt` が記載されているのに `file1.txt` が追跡対象になっていることを確認する
    2. `.gitignore` はまだ追跡されていないファイルを無視するための設定
11. リポジトリ内にもう 1 つのテキストファイル `file2.txt` を作成する現在の `git status` の出力を確認する
    1. `file2.txt`が追跡対象になっていないことを確認する
12. `git rm --cached` コマンドで `file1.txt` の削除をステージする
13. `git status` の出力を確認する
14. `file3.txt` というファイルを作成し `.gitignore` に `!file3.txt` という行を追加する
15. `git status` の出力を確認する
    1. 拡張子が無視されているにも関わらず`file3.txt`が追跡されていることを確認する

## 便利なコマンド

- `git rm`
- `git add`
- `git commit`
- `git commit -m`
- `git rm --cached`
