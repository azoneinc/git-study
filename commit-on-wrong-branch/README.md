# Commit on wrong branch

## セットアップ

1. `source setup.sh`（または PowerShell の場合は `.\setup.ps1`）を実行する

## 課題説明

あなたは master ブランチで作業している。作業内容をコミットした直後に緊急の対応が入ってしまった。現在の HEAD ではリリースできない状態なので 1 つ前のコミットから `quickfix` という新しいブランチを作成する。

緊急対応の変更を新しいブランチにコミットした結果、履歴が少し複雑になってしまった。現在のコミット履歴は以下の通り。

```text
         master
           |
           v
   A <---- B
   ^ \
   |  \--- C
remote     ^
           |
        quickfix
```

本来望ましい履歴は以下の通り。

```text
         remote
           |
           v
   A <---- C <---- B
                   ^
                   |
                  HEAD
```

このリポジトリは master ブランチを push することで自動リリースされるよう設定されていることとする。`master ブランチとして` C のコミットを push し、かつ B のブランチが master の HEAD となるように履歴を修正しなさい。

### 注意

この演習の環境設定では push ができないので上記の履歴通りになっていれば OK とする。

## タスク

1. `git log --oneline --graph --all` を使用してすべてのブランチとそのコミットを確認する
2. `quickfix` を master にリベースして master ブランチ上で `B` の前に `C` を配置する
3. master から新しいブランチ (`temp`) を作成して B 上での作業を継続できるようにする
   1. リリースのために master ブランチで `C` を push したい
   2. しかし `B` から `C` へ `reset --hard` すると `B` のコミットが消えてしまうので `temp` が必要
4. master を `C` にリセットする
5. `quickfix` ブランチを削除する
6. master を push する（演習では実際に実行できないのでした体でよい）
7. `temp` ブランチを master にマージ（ff-merge となる）して `temp` を削除する

## 便利なコマンド

- `git log --oneline --graph --all`
- `git switch <branch-name>`
- `git rebase <branch-name>`
- `git branch <branch-name>`
- `git reset --soft HEAD~`
- `git branch -d <branch-name>`
- `git merge <branch-name>`
