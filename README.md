# 国内使用 Git 克隆和上传仓库教程 ;)
解决git在国内无法使用的问题，此教程面向纯小白，用最简单的方式描述喵 ο(=•ω＜=)ρ⌒☆
## 为何使用 git
Github 是无法创建空文件夹的，另外通过浏览器上传文件到仓库不易管理
## 0.配置代理环境
1.以 Clash 为例，在科学的配置好了的环境后

2.在 General 界面中，打开 Allow LAN

3.查看 Service Mode 右侧小地球是否为绿色，如果不为绿色，点击最右侧 Manage，点击 install 安装虚拟网卡

4.安装成功后软件会自动重启，小地球随之便为绿色

5.打开 TUN Mode 和 System Proxy
## 1.下载 git
进入 [官网](https://gitforwindows.org/)  点击 Download 下砸
## 2.新建仓库
进入 Github 网站，点击右上角加号，点击 New repository，设置仓库名，点击最下方绿色按钮 Create Repository

新建完成后，进入仓库，点击绿色按钮 Code，复制那一串链接
## 3.配置本地仓库
进入需要上传的项目文件夹，右键点击 Open Git Bash Here，此时会在当前文件夹路径打开 Git 的命令行窗口

输入  git clone 步骤2复制的链接

此时在项目文件夹中会出现一个新的文件夹，文件夹名为在 Github 中建立的仓库时的仓库名

进入新的文件夹，将需要上传的文件或文件夹全部放到新文件夹中
## 4.上传文件的准备
1.输入 git config --global user.email " "

  引号中输入你 Github 的邮箱
  
2.输入 git add .

  这行意义为 上传当前文件夹所有文件（记住别把 . 给漏掉了哦）
  
3.输入 git commit -m " "

  引号中输入提交commit的注释
  
4.输入 git push origin 分支名

  此行中分支名指的是你 Github 中新建的仓库中的仓库名下方的那一个，有可能是 main 或者 master
  
  所以最终输入 git push origin main 或 git push origin master

  此时如果没有爆红应该就是上传成功啦，刷新仓库看看吧
## 可能情况
1. 在 clone 或 push 中 可能会出现 Git GUI 的弹窗，提示登陆 Github 账号，如果没有正确设置科学代理，可能不会有弹窗

2. 出现新报错时，可以试试 删除 clone 下来的文件 再重新 clone 和 push

3. 更多操作，可以查看 [官方文档](https://docs.github.com/zh/get-started/quickstart/hello-world)
