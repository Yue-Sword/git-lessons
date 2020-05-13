# GIT

## git项目提交到github

1. 创建本地文件夹git-lessons -> README.md

2. 在本地文件夹git-lessons下执行指令

   ```bash
   git init
   ```

3. 在github上创建一个同名git-lessons项目 ->  [LICENSE](https://github.com/Yue-Sword/git-lessons/blob/master/LICENSE

4. 设置远程仓库地址

   ```bash
   git remote add origin master git@github.com:Yue-Sword/git-lessons.git
   ```

5. 拉取并合并本地仓库与远程仓库： 

   ```bash
   git fetch
   git rebase origin master
   或
   git pull --rebase origin master
   ```

6. 提交本地代码

   > 第一次推送，需要添加 `--set-upstream` 或 `-u`，意思是设置已有的本地分支跟踪一个刚刚拉取下来的远程分支， 或者说要推送当前分支并将远程设置为上游 

   ```bash
   git add .
   git commit -m "xxx"
   git push --set-upstream origin master
   ```

   