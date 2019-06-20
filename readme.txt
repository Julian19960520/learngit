配置
$ git config --global user.name "Your Name"
$ git config --global user.email "email@example.com"

创建目录，进入目录，输出当前路径
$ mkdir learngit
$ cd learngit
$ pwd

初始化版本库，增加文件，删除文件，提交
$ git init
$ git add filename
$ git rm filename
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

撤销修改
$ git checkout -- filename		//就是让这个文件回到最近一次git commit或git add时的状态。
$ git reset HEAD <file>			//把暂存区的修改撤销掉（unstage），重新放回工作区：
场景1：当你改乱了工作区某个文件的内容，想直接丢弃工作区的修改时，用命令git checkout -- file。
场景2：当你不但改乱了工作区某个文件的内容，还添加到了暂存区时，想丢弃修改，分两步，第一步用命令git reset HEAD <file>，就回到了场景1，第二步按场景1操作。
场景3：已经提交了不合适的修改到版本库时，想要撤销本次提交，参考版本回退一节，不过前提是没有推送到远程库。

生成ssh钥匙
$ ssh-keygen -t rsa -C "2367852119@qq.com.com"

绑定本地库和远端库
$ git remote add origin git@github.com:michaelliao/learngit.git
$ git push -u origin master
$ git push origin master


