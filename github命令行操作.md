git version 列出版本号
本地文件夹
先添加到索引区
然后才能添加到库
git init 当前文件夹创建基础库
git config -1 查看当前git 库配置
git config --global user.name "名字"
git config --global user.email "897965465@qq.com"邮箱
git config --global color.ui true 控制台颜色
git help config 获取帮助
git status 查看文件状态是否提交
git add  index.html 把 index.html 提交到索引区
git commit -m "备注"  提交到本地库 
git log   列出提交历史
git log -1   列出2次提交历史
git log --oneline 一行显示
git log --oneline --graph --all 以树形展开分支
git log -p 详细显示
git log --stat 统计每次信息
git checkout -- (文件名)回复到未修改状态 未提交到索引区
git reset HEAD (文件名)回复到未修改状态 如果已经提交到索引区用这个
git diff 比较未到缓冲区文件
git diff --cached比较已经到缓冲区文件
git add . 把所有文件传到到索引区
git mv (文件名1) (文件名2)  改文件名
git  rm  stlet.css --cached 把索引区的stlet.css 删除
忽略文件 先创建.gitignore文件 想屏蔽谁就*（文件后缀）比如*.css 
git commit  --amend 提交并覆盖最后一次记录
首先 使用 git commit --amend 命令（修改最近一次提交的注释信息），会进入到vim 编辑器
按下字母键 c（此时进入编辑状态），可以开始修改注释信息了
按下Esc (退出编辑状态)； 接着连按两次大写字母Z，你会惊喜的发现，终于保存好退出来了！
git reset --hard HEAD~1 回到过去 回到已经提交仓库的版本(~1)是减去1的意思可以说任意数字
git reset --hard  edaf2cf 回到指定ID交仓库的版本  (edaf2cf) id 可用 git log 查看
git reflog  (-4列出4次记录)查找你移动多少次记录

git branch 查看当前分支 master是主分支 *号在哪个上就代表当前分支
git branch -a查看远程分支
git branch  (dev名字) 创建分支
git checkout dev 跳到 dev 分支
git merge (分支名)合并分支
git branch -d (分支名)删除分支
git checkout -b (分支名) 建立分支并且切换到分支
git remote add  (远程名称)  (远程地址) 添加远程仓库
git remote rm 移除添加的远程仓库 （名字）
git remote  -v 列出所有仓库
git push -u  （远程名称）  （分支名）上传代码
git push (仓库名) (分支名) --force 强制上代码
git clone 克隆 (远程地址)
git pull  拉取最新代码
git fetch 下到本地仓库不会合并cl