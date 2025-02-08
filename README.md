# Git 学習用コンテンツ

## 環境構築

![クイックスタート](/images/quickstart.gif)

1. 解きたい練習問題のフォルダへ移動する
2. そのフォルダ内の `README.md` を読んで演習の説明を確認する
3. `setup.sh` スクリプトを実行する
4. `exercise` ディレクトリへ移動して演習を始める

## 概要

`basic` から始まる演習は初心者向けでそれ以外の演習の難易度は高めです。

## 学習ロードマップ

1. [basic-commits](basic-commits/README.md) - 基本的なコミットの作成
1. [basic-staging](basic-staging/README.md) - ステージ（インデックス）との対話
1. [basic-branching](basic-branching/README.md) - ブランチ作成への最初の一歩
1. [ff-merge](ff-merge/README.md) - 単純なマージ
1. [3-way-merge](3-way-merge/README.md) - 複数の分岐したブランチを含む基本的なマージ
1. [merge-conflict](merge-conflict/README.md) - 分岐ブランチの基本的なマージ
1. [merge-mergesort](merge-mergesort/README.md) - 実際のコードを用いたマージコンフリクト
1. [rebase-branch](rebase-branch/README.md) - マージの代替手段としてリベースを使用
1. [basic-revert](basic-revert/README.md) - 変更を取り消すためにリバートを使用
1. [reset](reset/README.md) - リセットの 3 つのモードを確認してください
1. [amend](amend/README.md) - 以前のコミットの修正
1. [reorder-the-history](reorder-the-history/README.md) - コミットの順番が最適でなかった場合の修正
1. [squashing](squashing/README.md) - コミットのまとめ方
1. [Rebase using autosquash](./rebase-interactive-autosquash/README.md) - autosquash を利用したリベースコマンドの使用
1. [basic-stashing](basic-stashing/README.md) - スタッシングへの最初の一歩
1. [ignore](ignore/README.md) - `.gitignore`ファイルの基本的な使い方および `git rm` の使用
1. [git-tag](git-tag//README.md) - タグの使用

## 課題

### [commit-on-wrong-branch](commit-on-wrong-branch/README.md)

誤ってプッシュされていないコミットを誤ったブランチに入れてしまった場合、作業を開始する前にどのように別のブランチへ _移動_ させるか。

### [commit-on-wrong-branch-2](commit-on-wrong-branch-2/README.md)

誤ったブランチに誤ってコミットしてしまった場合の対処法に関する演習。

### [save-my-commit](save-my-commit/README.md)

誤ってコミットを削除してしまった場合これを救出する方法を試してみてください。reflog を使用します。

### [advanced-rebase-interactive](advanced-rebase-interactive/README.md)

インタラクティブリベースを用いた高度な操作。

## 発展課題

### [reverted-merge](reverted-merge/README.md)

マージをリバートしましたがマージ先ブランチに修正が加えられた後、マージ時の変更と新しい修正の両方を反映させたい場合。

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
