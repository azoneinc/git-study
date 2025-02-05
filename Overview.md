# 学習用コンテンツ概要

## 環境構築

1. [configure-git](configure-git/README.md) - 基本的な設定手順

## 学習ロードマップ

1. [basic-commits](basic-commits/README.md) - 基本的なコミットの作成
2. [basic-staging](basic-staging/README.md) - ステージ（インデックス）との対話
3. [basic-branching](basic-branching/README.md) - ブランチ作成への最初の一歩
4. [ff-merge](ff-merge/README.md) - 単純なマージ
5. [3-way-merge](3-way-merge/README.md) - 複数の分岐したブランチを含む基本的なマージ
6. [merge-conflict](merge-conflict/README.md) - 分岐ブランチの基本的なマージ
7. [merge-mergesort](merge-mergesort/README.md) - 実際のコードを用いたマージコンフリクト
8. [rebase-branch](rebase-branch/README.md) - マージの代替手段としてリベースを使用
9. [basic-revert](basic-revert/README.md) - 変更を取り消すためにリバートを使用
10. [reset](reset/README.md) - リセットの 3 つのモードを確認してください
11. [basic-cleaning](basic-cleaning/README.md) - ワークスペースのクリーンアップ
12. [amend](amend/README.md) - 以前のコミットの修正
13. [reorder-the-history](reorder-the-history/README.md) - コミットの順番が最適でなかった場合の修正
14. [squashing](squashing/README.md) - コミットのまとめ方
15. [advanced-rebase-interactive](advanced-rebase-interactive/README.md) - インタラクティブリベースコマンドの使用
16. [Rebase using autosquash](./rebase-interactive-autosquash/README.md) - autosquash を利用したリベースコマンドの使用
17. [basic-stashing](basic-stashing/README.md) - スタッシングへの最初の一歩
18. [ignore](ignore/README.md) - `.gitignore`ファイルの基本的な使い方、および `git rm` の使用
19. [submodules](submodules/README.md) - サブモジュールが非推奨な理由を知る
20. [git-tag](git-tag//README.md) - タグの使用

## 課題

### [commit-on-wrong-branch](commit-on-wrong-branch/README.md)

誤ってプッシュされていないコミットを誤ったブランチに入れてしまった場合、作業を開始する前にどのように別のブランチへ _移動_ させるか。

### [commit-on-wrong-branch-2](commit-on-wrong-branch-2/README.md)

誤ったブランチに誤ってコミットしてしまった場合の対処法に関する演習。

### [reverted-merge](reverted-merge/README.md)

マージをリバートしましたがマージ先ブランチに修正が加えられた後、マージ時の変更と新しい修正の両方を反映させたい場合。

### [save-my-commit](save-my-commit/README.md)

誤ってコミットを削除してしまった場合これを救出する方法を試してみてください。reflog を使用します。

### [detached-head](detached-head/README.md)

Git は「detached HEAD」状態にあると警告します。どう対処しますか？

## 発展課題

### [git-attributes](git-attributes/README.md)

.gitattributes ファイルを使用してテキストファイルの改行コードやバイナリファイルの差分表示方法など、Git がファイルをどのように扱うかを指定できます。

### [Bad-commit](bad-commit/README.md)

`git bisect`を使用して悪いコミットを見つける。

### [bisect](bisect/README.md)

`git bisect`を使用する別の演習。

### [pre-push](pre-push/README.md)

Git フックの使用に関する簡単な演習。

### [Investigation](investigation/README.md)

Git リポジトリ内で何が起こっているかを発見しその内部構造を把握する。

### [Objects](objects/README.md)

Git 内部構造に関する小さな演習。

### [merge-driver](merge-driver/README.md)

カスタムマージドライバーの定義。

### [rebase-exec](rebase-exec/README.md)

`git rebase --exec`を使用して各コミットでテストを実行。
