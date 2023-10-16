克隆存储库:

# git clone

获取该目录中长格式的文件列表:

# ls -l

创建一个分支:

# git branch chenqingsong

执行以下命令看到 Git 创建了新分支:

# git branch

切换到 chenqingsong 分支:

# git checkout chenqingsong

执行以下命令来标记你对文件所做的更改:

# git add README.md

提交更改:
[chenqingsong 8b940f8] secondDaily
1 file changed, 28 insertions(+), 5 deletions(-)

# git commit -m "firstDaily"

本地更改推送到分支的远程存储库:
–set-upstream 告诉 Git 在本地存储库和远程存储库之间为此分支形成跟踪链接。

# git push --set-upstream chenqingsong

删除:

# rm -rf chenqingsong

显示工作树的当前状态——即您正在处理的目录中的文件集合:

# git status

比较同一文件的两个版本:

# git diff

# git diff --staged

将所有更改添加到暂存区域:

# git add .

查看 git 日志:

# 查看 git 日志

显示提交的实际差异:

# git log -p

git 重置 :

# git reset HEAD

git reset HEAD <filename>允许您将暂存环境恢复到最后一个提交状态
git mv 在一个动作中移动文件并分阶段更改
git rm 从存储库中删除文件，并在一个操作中再次分阶段更改
使用 git reset HEAD <filename> 恢复已删除和分阶段的文件，然后 git checkout HEAD <filename>
git log -2 要查看的提交数量 2
git log --oneline 查看存储库历史记录的更紧凑视图

存储库的图形视图:

# git log --graph

# git log --oneline --graph

展示它所知道的一切的完整历史记录:

# git log --oneline --graph --all

查看谁已提交到此存储库:

# git shortlog

该文件所有完整提交消息:

# git log --oneline <chen>

git log 本身显示了当前 HEAD 的祖先承诺的基本视图。
git log -p 显示提交的差异。
git log -n 显示最后 n 个提交。
git log --oneline 显示短散列和提交消息的简明视图。
可以在 git log 上堆叠选项，如 git log -8 --oneline，以压缩形式显示最后 8 个提交。
git log --graph 显示存储库的粗糙但可行的图形表示。
git log --all 显示存储库中其他分支的提交，而不仅仅是当前 HEAD 的祖先。
git shortlog 显示按时间顺序按作者分组的提交摘要。
git log --author="<authorname>"允许您搜索特定作者的提交。
git log --grep="<term>"允许您搜索特定术语的提交消息。
git log <path/to/filename>将只向您显示与该文件关联的提交。
git log <directory>将向您显示特定目录中文件的提交。
git log --stat 显示了每个提交中更改的范围和规模的漂亮概述。
git log -S"<term>"允许您搜索特定术语的提交更改集的内容。

删除分支:

# git branch -d chenqingsong

使用 git branch <branchname>创建一个分支。
使用 git branch 查看所有本地分支。
使用 git checkout <branchname>切换到本地分支，或签出和跟踪远程分支。
使用 git branch -d <branchname>删除本地分支。
使用 git branch --all 查看所有本地和远程分支。
origin，和 main 一样，只是一个方便的约定，是远程存储库 URL 的别名。
使用 git checkout -b <branchname>一举创建并切换到本地分支。

git log <theirs> --not <ours>显示您要合并的分支上哪些提交，这些提交尚未在您的分支中。
git merge <theirs>将“他们的”分支上的提交合并到“我们的”分支中。

Git 从 main 分支中获取更改，并将远程存储库（origin）与您的更改同步:

# git push origin main

更改从遥控器拉入本地:

# git pull origin

设置 git 用户名和电子邮件
git config --global user.name "your-username-here"
git config --global user.email "youremail@domain.com"

