# 作業フロー
作業してからコミット/プッシュするまでにできること。

```txt
/Local < Working..
┴─ 
staging
┬─ 
↓
├── `$ git reset` - 編集を削除
├── `$ git stash` - 編集を退避
┴─ 
$ git commit
┬─ 
↓
├── `$ git commit --amenda` - 前回のコミットを編集
├── `$ git rebase` - コミットを編集
├── `$ git` 
├── `$ git cherry pick` - コミットをブランチ間で移動
┴─ 
$ git push
┬─ 
↓
┴
/Origin
```

:joy:
