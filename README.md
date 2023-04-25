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
- git log
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
