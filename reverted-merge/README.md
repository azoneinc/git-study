# Reverted merge

## 課題説明

あなたのチームは別のチームが管理する library-1.2.3 を利用している。ある時点であなたのチームは新バージョン library-1.2.4 を統合する。
慎重を期すためこの作業は `integrate-library-1.2.4` ブランチで行う。

しかしマージ後にライブラリでバグが発見される。このバグは別のチームによって修正されなければならない。バグが本番環境にリリースされるのを防ぐため、あなたはマージコミットをリバートすることにする。

## セットアップ

1. Run `source setup.sh`（PowerShell の場合は `.\setup.ps1`）

## タスク

1. マージコミットをリバートする
   - コンフリクトを解消するため、`mymodule.txt` にどの機能を含めるべきか判断する必要がある
   - 機能 X を含めるか否かはコミット時期で判断できる
   - 機能 Y は旧ライブラリバージョンで動作していると仮定してよい
2. ライブラリチームの立場をとり `integrate` ブランチ上でライブラリのバグを修正する（例： `lib.txt` を変更する）
3. 次にブランチから master に変更を取り込む方法を検証する  
   最初にマージを試すと、`lib.txt` は期待通りに変更されるが、`mymodule.txt` は変更されない  
   理由の詳細については、以下の gist を参照する： [Reverting a faulty merge](https://github.com/git/git/blob/master/Documentation/howto/revert-a-faulty-merge.txt)  

   > reverting a merge commit also  
   > undoes the _data_ that the commit changed, but it does absolutely  
   > nothing to the effects on _history_ that the merge had  
   >
   > So the merge will still exist, and it will still be seen as joining  
   > the two branches together, and future merges will see that merge as  
   > the last shared state  
4. `reset --hard` を使ってマージを取り消す  
5. リバートをリバートし再度マージを試みる  

## 便利なコマンド

- `git revert -m 1 <merge-sha1>`
- `git log --oneline --graph --all`
- `git add <file-name>`
- `git revert --continue`
- `git switch <branch-name>`
- `git merge <branch-name>`
- `git reset --hard <sha1>`
- `git revert <sha1>`
