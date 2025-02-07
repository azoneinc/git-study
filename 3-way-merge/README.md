# 3-Way Merge

## セットアップ

1. `source setup.sh` を実行する（または PowerShell では `.\setup.ps1` を実行する）

## 課題

1. greeting というブランチを作成して切り替える
1. greeting.txt を任意に編集するしてコミットする
1. master ブランチに戻る
1. README.md ファイルを新規作成し任意の内容でコミットする
1. `git log --oneline --graph --all` の出力を確認する
1. greeting ブランチを master ブランチにマージする
1. `git log --oneline --graph --all` の出力を確認する
1. `Merge branch 'greeting'`というメッセージで作成されたマージコミットが自動で作られていることを確認する

## 便利なコマンド

- `git branch`
- `git branch <branch-name>`
- `git branch -d <branch-name>`
- `git switch <branch-name>`
- `git switch -c <branch-name>`
- `git branch -v`
- `git add`
- `git commit`
- `git commit -m`
- `git merge <branch-name>`
- `git diff <branchA> <branchB>`
- `git log --oneline --graph --all`
