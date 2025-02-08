# Save my commit

このリポジトリでは履歴の何処かで `holygrail.txt` を追加した。しかし誤って `master` ブランチを初期コミットに hard リセットしてしまった。どうにかして変更を復元する方法はないか。

## セットアップ

1. `source setup.sh` を実行する (PowerShell の場合は `.\setup.ps1`)

## タスク

1. `git log` を使用して履歴が短いことを確認する
2. `ls` を使用して `holygrail.txt` がワークスペースに存在しないことを確認する
3. `git reflog` を使用して `holygrail.txt` を追加したコミットを見つける
4. `git reset --hard` を使用して履歴と作業内容を回復する
5. `git log` と `ls` を使用して回復した作業内容を確認する
6. `git reset --hard initial-commit` を実行して解決策を取り消す
7. `git cherry-pick` を使用して `holygrail.txt` を復元する
8. reset を使用した解決策と履歴およびワークスペースを比較する

## 関連 Git コマンド

- `git reflog`
- `git cherry-pick`
- `git reset --hard`
- `git log`
