# 常用git指令

### 创建版本库
~~~
  创建空文件夹  

  初始化创建仓库           git init  

  添加文件到git仓库        git add .  git commit -m " "

  查看仓库状态             git status  

  查看内容修改             git diff  

  查看提交历史             git log  
~~~

### 远程仓库管理
~~~
  克隆远程仓库             git clone https://github.com/zylxxb/github.git

  添加文件                 git add .   git commit -m " "

  推送到远程仓库           git push origin master
~~~

### 远程仓库分支管理
~~~
  查看分支                   git branch

  创建分支                   git checkout zylxxb_develop

  创建+切换分支              git checkout -b zylxxb_develop

  切换分支                   git checkout master/zylxxb_develop

  删除分支                   git branch -d zylxxb_develop

  合并分支(master分支合并)    git merge zylxxb_develop
~~~
