# git

```
"# git" >> README.md            生成README文件
git remote add origin https://  添加远程仓库
                                -v显示远程仓库列表
git push -u origin master       推送并设置origin为默认主机
                                -f命令去强制提交
git pull                        拉取

git init                        初始化
git status                      查看状态
git add                         添加到暂存区
git commit -a -m                将暂存区的修改提交到仓库
                                -a跳过暂存区
                                -m直接在命令行输入注释,不打开编辑器
                                --amend替换最后一次提交
git rebase -i HEAD~3            合并commmit -i的意思是--interactive 后面的参数是指定编辑区间
                                进如编辑模式后 pick 为保留的 squash 为需要合并的
git diff --staged               查看尚未暂存的文件更新了哪些部分
                                --staged查看已暂存的将要添加到下次提交里的内容
git reset                       撤销操作 HEAD~2 回退到前两个版本
                                --soft 还原 HEAD
                                --mixed 还原 HEAD、Index 默认
                                --hard 还原 HEAD、Index、Working Directory 彻底回退到某个版本，本地的源码也会变为上一个版本的内容
git branch -d                   查看分支 后面跟名称创建对应名称的分支
                                -d删除分支
git checkout -b                 切换分支
                                -b创建并切换分支
git merge                       合并某分支到当前分支上
git reflog                      显示所有commit
git log --pretty=format:"%h %an %ad %s" --date=format:"%Y-%m-%d %H:%M:%S"
                                查看历史记录
                                --pretty=format输出格式包括 oneline，short，full，fuller 和 format（后跟指定格式）
                                %H 提交对象（commit）的完整哈希字串
                                %h 提交对象的简短哈希字串
                                %T 树对象（tree）的完整哈希字串
                                %t 树对象的简短哈希字串
                                %P 父对象（parent）的完整哈希字串
                                %p 父对象的简短哈希字串
                                %an 作者（author）的名字
                                %ae 作者的电子邮件地址
                                %ad 作者修订日期（可以用 --date= 选项定制格式）
                                %ar 作者修订日期，按多久以前的方式显示
                                %cn 提交者（committer）的名字
                                %ce 提交者的电子邮件地址
                                %cd 提交日期
                                %cr 提交日期，按多久以前的方式显示
                                %s 提交说明
```
