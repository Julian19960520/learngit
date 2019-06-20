配置
$ git config --global user.name "Your Name"
$ git config --global user.email "email@example.com"

创建目录，进入目录，输出当前路径
$ mkdir learngit
$ cd learngit
$ pwd

初始化版本库，增加文件，提交
$ git init
$ git add filename.txt
$ git commic -m"message"

查看版本库状态，文件差异
$ git status
$ git diff filename

版本回退
$ git reset --hard HEAD^
$ git reset --hard eb2c75e

Log命令
$ git log --pretty=oneline
$ git reflog
