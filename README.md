# 目錄
* [GIT基本指令](#GIT基本指令)
* [標籤](#標籤)
* [Branch相關指令](#Branch相關指令)


# GIT基本指令

## 第一次登陸GIT必須登錄

**登陸使用者名稱**

`$ git config --global user.name "<使用者名字>"`

**登陸電子郵件**

`$ git config --global user.email "<電子信箱>"`


## 建立數據庫

`$ git init`


## 遠端數據庫

**新增遠端數據庫**

`$ git remote add [remote name] [url]`

**將數據庫的指定分支下載到本地**

`$ git pull [remote name] [branch name]`

**移除遠端數據庫**

`$ git remote add [remote name] [url]`


## 上傳資料到遠端

**加入commit清單**

`$ git add "[data name or path]"`

**更新本地修改過的資料**

`$ git add -u`

or 

`$ git add .`


**提交版本**

`$ git commit -m [remote name]`

**上傳到遠端**

`$ git push [remote name] [branch name]`

## 檢視提交的歷史記錄及UID

`$ git log --oneline`


# 標籤

**查看標籤**

`$ git tag`

**在 commit 點上新增標籤**

`$ git tag [tag name] [?] -a -m "tag name"`

**移除標籤**

`$ git tag -d [tag name]`


# Branch相關指令

**建立分支**

`$ git branch [branch name]`

**刪除分支**

`$ git branch -d [branch name]`

**切換分支**

`$ git checkout [branch name]`

**創建分支並切換**

`$ git checkout -b [branch name]`

**移除遠端分支**

`$ git push [remote name] :[branch name]`

**重新命名分支名稱**

`$ git branch -m [branch name] [newbranch name]`

**下載所有分支**

`$ git pull --all`

**合併分支(會產生新的commit)**

`$ git merge [branch name]`

**合併分支(複製接上的概念)**

`$ git rebase [branch name]`

**查看分支**

`$ git branch`

**查看所有分支**

`$ git branch -a`
