ローカル環境でのGit
=====

リモートリポジトリーの作成
----
```bash
# 1. 配置するディレクトリーに移動
$ cd PATH/TO/REMOTE
# 2. 初期化
$ git init --bare
```

リモートからクローンする
----
```bash
# 1. 作業ディレクトリに移動
$ cd PATH/TO/LOCAL
# 2. クローンする
$ git clone PATH/TO/REMOTE
# 2-b 名前を指定する場合
$ git clone PATH/TO/REMOTE NAME
```

既存の作業ディレクトリに紐つける
----
```bash
# 1. 作業ディレクトリに移動 
$ cd PATH/TO/LOCAL
# 2. 初期化
$ git init
# 3. リモートとの紐付け
$ git remote add NAME PATH/TO/REMOTE

# - 確認
$ git remote -v
```

リモートを解除
-----
```bash
$ git remote rm NAME
```

参考
- [Git のリモートリポジトリを Dropbox 上に作成して共有する](http://m.designbits.jp/13061220/)
- [私の使うGitコマンドまとめ 基本コマンド編](http://naokirin.hatenablog.com/entry/20111201/1322576109)
- [はじめてのgitレビューを読んでinstallしたけど使っていないgitの使い方を学ぶ](http://d.hatena.ne.jp/Akira51/20101028/1288257595)

