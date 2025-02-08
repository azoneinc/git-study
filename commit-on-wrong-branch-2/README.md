# Commit on wrong branch II

## 課題説明

あなたは `new-feature` ブランチで新機能を開発している。既に機能の一部が実装できたところで `master` ブランチに重大なバグが発生し緊急で対応した。バグ修正後に新機能の開発を続ける。

更に機能を追加しコミットした後、そのコミットが `new-feature` ブランチではなく `master` ブランチにコミットされていることに気づいた。

以下の内容を満たすコミットログに修正せよ。

- 誤って `master` にコミットした内容を `new-feature` に取り込む
- master から機能追加のコミットを取り除く
- `new-feature` へ `master` に適用したバグ修正のコミットを取り込む

## セットアップ

1. Run `source setup.sh`（PowerShell の場合は `.\setup.ps1`）

## タスク

### 差分を stash する方法

1. `git reset HEAD~1` で現在のコミット内容を維持したまま 1 つ前の履歴（`Fix bug` というコメントのコミット）に戻る
2. `git stash` でコミットされていない変更点をスタッシュする
   1. これでバグ修正後の追加機能の開発内容をスタッシュとして分離できた
3. `new-feature` に移動する
4. スタッシュを適用しコミットする
   1. スタッシュ適用時にコンフリクトが発生するので手動または `git mergetool` で解決する
5. `master` のバグ修正のコミットを `git cherry-pick` で取り込む
   1. master を new-feature にリベースするのでもよい

### cherry-pick で取り込む方法

1. `new-feature` に移動する
2. `git cherry-pick` で `master` に誤ってコミットされた追加機能のコミットを取り込む
   1. コンフリクトが発生するので手動または `git mergetool` で解決し `git add .`→`git cherry-pick --continue` する必要がある
3. `master` に移動し `git reset --hard HEAD~` で追加機能のコミットを削除する
4. `new-feature` に移動する
5. `master` のバグ修正のコミットを `git cherry-pick` で取り込む
   1. master を new-feature にリベースするのでもよい

## 便利なコマンド

- `git reset HEAD~1`
  - 現在のブランチを 1 つ前に戻す
  - これにより最新のコミットがブランチから削除される
- `git stash`
  - ブランチを切り替えられるよう一時的に変更内容を保存する
- `git cherry-pick`
  - 現在のブランチ上のコミットから変更セットを追加する
