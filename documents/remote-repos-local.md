# ローカル環境にリモートリポジトリーを設置する

## 手順

### 1. リモートリポジトリーの作成

```sh
$ cd PATH/TO/REMOTE             # 作成する任意のフォルダに移動
$ git init --bare               # リモートリポジトリーを作成   
```

### 2. ローカル環境の作成

#### 2-1. リモートからクローンする場合

```sh
$ cd PATH/TO/LOCAL              # ローカル環境を作成するフォルダに移動
$ git clone PATH/TO/REMOTE      # リモートからクローンする
# (名前を指定してクローンする場合は次のようにします)
$ git clone PATH/TO/REMOTE NAME 
```

#### 2-2. 既存の作業ディレクトリに紐付ける場合

```sh
$ cd PATH/TO/LOCAL              # ローカル環境の作業フォルダに移動
$ git init                      # Git を初期化
$ git remote add NAME PATH/TO/REMOTE # リモートに紐つける
```

### 3. 確認

```sh
$ git remote -v
```


### 4. リモートを解除する
```sh
$ git remote rm NAME
```


## 参考リンク

- [Git のリモートリポジトリを Dropbox 上に作成して共有する](http://m.designbits.jp/13061220/)
- [私の使うGitコマンドまとめ 基本コマンド編](http://naokirin.hatenablog.com/entry/20111201/1322576109)
- [はじめてのgitレビューを読んでinstallしたけど使っていないgitの使い方を学ぶ](http://d.hatena.ne.jp/Akira51/20101028/1288257595)

