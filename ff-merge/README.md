# Fast-forward Merge

## セットアップ

1. `source setup.sh` を実行する（PowerShell では `.\setup.ps1` を実行する）

## 課題

1. `feature/uppercase` という (feature) ブランチを作成する
2. このブランチに切り替える
3. `git status` の出力は何か
4. greeting.txt を編集して大文字の挨拶文にする
5. greeting.txt ファイルをステージングエリアに追加してコミットする
6. `git branch` の出力は何か
7. `git log --oneline --graph --all` の出力は何か
8. `master` ブランチに切り替える
   1. feature ブランチにあるすべての変更を master ブランチに取り込みたい
   2. コマンド 'git merge[branch name]' は引数として 1 つのブランチを取りそのブランチの変更を取得する
   3. HEAD が指すブランチ（現在チェックアウトされているブランチ）が指定したブランチの変更を取り込むように更新される
9. `cat` を使用して挨拶文の内容を確認する
10. ブランチを比較する
11. ブランチをマージする
12. `cat` を使用して挨拶文の内容を確認する
13. uppercase ブランチを削除する

## 便利なコマンド

- `git branch`
- `git branch <branch-name>`
- `git branch -d <branch-name>`
- `git switch`
- `git branch -v`
- `git add`
- `git commit`
- `git commit -m`
- `git merge <branch>`
- `git diff <branchA> <branchB>`
- `git log --oneline --graph --all`
