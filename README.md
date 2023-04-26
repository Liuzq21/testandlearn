# testandlearn
lzq初期学习github
https://zhuanlan.zhihu.com/p/369486197
## 了解Github
- merge
- fork
- clone
- watch
- pull request
等

## Git使用
git官网
https://git-scm.com/download
下载git并安装
https://blog.csdn.net/mukes/article/details/115693833

### 常用git命令
- git status
- git init
- git add <filename>  // 本质上仅提交到缓冲区里面
- git commit -m "text commit"  // 正式提交仓库，-m后面输入的是本次提交的说明，可以输入任意内容，当然最好是有意义的，这样你就能从历史记录里方便地找到改动记录。
- git log  ； git log --pretty=oneline
- git branch 
- git branch a // 创建a分支
- git checkout a // 切换到a分支
- git merge a // 将a分支合并到当前分支
- git branch -d a 删除
- git tag v1.0 // 为当前分支添加标签v1.0 用git tag 查看

### 在本地创建版本库
找个目录，右键，选择git bash
1. 通过git init命令把这个目录变成Git可以管理的仓库，ls -ah可以看见。
2. git add <filename> 把这个文件加进来
3. 用命令git commit告诉Git，把文件提交到仓库
注意：git命令均要在仓库下执行，需要add的文件也要在仓库目录下。
### 查看、回退版本库内容
1. 用git status 看仓库状态
2. git diff 查看上次修改内容
3. git reset --hard HEAD^  // HEAD 表示当前版本，HEAD^ 表示上一个版本，HEAD^^ 表示上上个，HEAD~100 表示上100个
4. git reset --hard <版本号> // 可以到达指定的版本
5. 要是一不小心忘记了版本号然后又关闭了终端导致最新版本又没记住可是又想回到最新版本，可以git reflog查看之前使用过的命令，找到最新版本的版本号
6. git工作原理：程序员在工作区改文件，add对文件的修改进暂存区，commit修改至分支。所以git管理的是对文件的修改。
7. 撤销修改：git checkout -- <file>  // 将文件回到最近一次git commit或git add时的状态；
8. 撤销修改：git reset HEAD <file>  // 把暂存区的修改撤销掉，重新返回工作区
9. 删除文件：git rm <file> ; 
10. 恢复文件：git checkout -- <file>其实是用版本库里的版本替换工作区的版本，无论工作区是修改还是删除，都可以“一键还原”。

### 远程仓库
