# Basic Branching

## セットアップ

1. `source setup.sh` を実行する（PowerShell では `.\setup.ps1`）

## 課題

この度はブランチを少しいじって、git におけるブランチの軽量さを示す。
`git switch` を使うとあるブランチから別のブランチへ切り替えることができる。

1. この演習に関連する 2 つのブランチを確認するために `git branch` を使用する
2. 現在どのブランチにいるか
3. 新しいブランチ _mybranch_ を作成するために `git branch mybranch` を使用する
4. 新しく作成されたブランチを確認するためにもう一度 `git branch` を使用する
5. 新しいブランチに切り替えるため `git switch mybranch` を使用する
6. _master_ ブランチと新しく作成したブランチ間を切り替えたとき、`git status` の出力はどのように変化するか
7. 2 つのブランチ間を切り替えたとき、ワークスペースはどのように変化するか
8. 続行する前に、_mybranch_ ブランチ上にいることを確認する
9. 自分の名前が書かれた `file1.txt` というファイルを作成する
10. ファイルを追加してこの変更をコミットする
11. 新しいコミットを指すブランチを確認するために `git log --oneline --graph` を使用する
12. _master_ ブランチに戻る
13. `git log --oneline --graph` を使用して _mybranch_ ブランチで行ったコミットが _master_ ブランチには存在しないことを確認
14. `file2.txt` という新しいファイルを作成してそのファイルをコミットする
15. `git log --oneline --graph --all` を使用して各ブランチが新しいコミットを指しており 2 つのブランチが異なるコミットを持っていることを確認する
16. 自分のブランチ _mybranch_ に切り替える
17. ワーキングディレクトリがどうなったか確認し `file2.txt` が存在しているか確認
18. 2 つのブランチ間の違いを確認するために `git diff mybranch master` を使用する

## 便利なコマンド

- `git switch`
- `git switch -c`
- `git log --oneline --graph`
- `git branch`
- `git diff`
