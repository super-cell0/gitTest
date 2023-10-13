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
