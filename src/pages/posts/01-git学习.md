<img src="https://s21.ax1x.com/2025/03/26/pEDBY26.jpg" alt="pEDBY26.jpg" border="0" />



> 记录我的学习旅途**

## **今日份学习：Git使用**

**这是个Git教学网站，适合初学者学习Git相关指令**  
<https://liaoxuefeng.com/books/git/introduction/index.html> 

****

### **windows安装Git**

- ###### 详细安装教程<https://blog.csdn.net/mukes/article/details/115693833>

- 安装完成后配置Git

  ```
  $ git config --global user.name "Your Name"
  $ git config --global user.email "email@example.com"
  ```

### **相关命令**

- 创建版本库

  ```
  $ cd /e/git
  $ mkdir learngit
  $ cd learngit
  $ pwd
  /E/git/learngit
  ```

- 初始化仓库

  ```
  $ git init
  Initialized empty Git repository in /E/git/learngit/.git/
  ```

****

```
$ git add read.txt //将文件添加到Git仓库
$ git rm test.txt //将文件从Git仓库删除
$ git commit -m "wrote a read file" //将文件提交到Git仓库
$ git status //查看仓库当前状态
$ git diff read.txt //查看difference
$ git log //查看git历史记录($ git log --pretty=oneline)
$ git reset --hard HEAD^ //版本回退(git reset --hard HEAD~1)
//$ git reset --hard 1094a(版本id)
$ git reflog //记录每一次命令
$ git diff HEAD -- read.txt //查看工作区和版本库里面最新版本的区别
$ git checkout -- read.txt //丢弃工作区的修改
$ git reset HEAD readme.txt //撤销暂存区的修改
$ ssh-keygen -t rsa -C "youremail@example.com" //创建ssh-key
$ git remote add origin xx //关联本地与远程仓库
git push -u origin master //将本地库内容推送至远程仓库
$ git remote -v //查看远程库信息
$ git remote rm origin //解除origin远程库绑定
$ git clone xx //克隆仓库
$ git config --global color.ui true //让Git显示颜色
```

