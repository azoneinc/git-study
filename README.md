# Git 学習コンテンツ

Git の概念、基本操作を理解している人を対象としています。（commit、fetch、pull、push ができるくらい）未経験や基本的な操作が不安な方は以下の初級用のコンテンツか Udemy などで基本を理解してから取り組んだ方が良いかもしれません。

* [サル先生の Git 入門](https://backlog.com/ja/git-tutorial/intro/01/)
  * 入門編と発展編を取り組んでください

## 注意

本講座では Git がもつ本来の機能や操作を理解し実践できるようになることを目的としています。 `SourceTree`や`Fork`などの Git クライアントツールを使用せずコマンドラインで取り組んでください。（後半の課題はコマンドを利用することでしか解決できない問題が多く含まれています）

## 座学

以下の書籍を参考に`自身でコマンドラインから操作`することで手を動かして学習してください。

* [Pro Git book](https://git-scm.com/book/ja/v2)
  * 1〜3 章
    * 全て対象
  * 4 章
    * 操作は必要ないが理解は必要
  * 7 章
    * 7.11〜14 以外全て対象（7.11〜14 も学ぶ価値はある）

## 課題

[Easy](#easy)と[Middle](#middle)まで完了して本講座を修了とします。[Advance](#advance)に関しては余力があれば取り組んでください。

### 課題の環境構築方法

![クイックスタート](/images/quickstart.gif)

1. 解きたい練習問題のフォルダへ移動する
2. そのフォルダ内の `README.md` を読んで演習の説明を確認する
3. `setup.sh` スクリプトを実行する
4. `exercise` ディレクトリへ移動して演習を始める

### Easy

非常に簡単なものも含まれているので課題を読んで必要ないと思ったものは飛ばしても構いません。

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
11. [amend](amend/README.md) - 以前のコミットの修正
12. [reorder-the-history](reorder-the-history/README.md) - コミットの順番が最適でなかった場合の修正
13. [squashing](squashing/README.md) - コミットのまとめ方
14. [rebase-interactive-autosquash](./rebase-interactive-autosquash/README.md) - autosquash を利用したリベースコマンドの使用
15. [basic-stashing](basic-stashing/README.md) - スタッシングへの最初の一歩
16. [ignore](ignore/README.md) - `.gitignore`ファイルの基本的な使い方および `git rm` の使用
17. [git-tag](git-tag//README.md) - タグの使用

### Middle

Git の操作において一般的に遭遇するケースを想定した課題です。どの課題もコマンド 1 つで直せるような簡単な状況ではありません。
コマンドを丸暗記する必要はありませんが Git でできることを理解し、必要な操作を自分で組み立てられるようにしましょう。（その過程でコマンドは自然と身につきます）

### [commit-on-wrong-branch](commit-on-wrong-branch/README.md)

誤って feature ブランチではなく master ブランチにコミットしてしまった場合にコミットを _移動_ させる方法。

### [commit-on-wrong-branch-2](commit-on-wrong-branch-2/README.md)

誤ったブランチにコミットしてしまった場合の対処法。

### [save-my-commit](save-my-commit/README.md)

誤ってコミットを削除してしまった場合に復元する方法。

### [advanced-rebase-interactive](advanced-rebase-interactive/README.md)

インタラクティブリベースを用いた高度な操作。

### Advance

これらの課題は遭遇することが稀なケースや高度な Git の操作方法です。これらの操作はできなくとも実務で困ることはまずありません。
Git の深淵に触れてみたい場合は是非チャレンジしてみてください。

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
