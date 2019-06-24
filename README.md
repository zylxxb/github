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
  
  克隆远程仓库项目分支      git clone -b zylxxb_develop https://github.com/zylxxb/github.git
  
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

  删除远程仓库分支(推送空分支) git push origin :zylxxb_develop
~~~

### 解决本地仓库push远程仓库每次都要重复输入密码的问题

>  方法一： 执行一命令 git config --global credential.helper store后，下次输入账号密码会默认记住

>  方法二： 设置git本地仓库的用户名和密码、油箱与远程仓库(github)一致

~~~
   // 设置
   git config --global user.name "xxx"

   git config --global user.email "xxx"

   git config --global user.password "xxx"

   // 查看
   git config user.name/email/password
~~~

### 解决本地仓库github下载的项目文件配置问题
~~~
   node-modules安装：    npm install
   sass编译模块：        npm install node-sass@lates
~~~
