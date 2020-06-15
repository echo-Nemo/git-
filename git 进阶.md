# git:全量 （每一个版本包含所有的文件，时刻保持数据的完整性）
# git的状态
	* 已修改: modified
	* 已暂存：staged
	* 已提交：commited
	
# git log
	* 查看提交日志
	
# git log -最近提交的数字
	* git log -2
	
# linux下的指令
	* ctrl +a :回到头
	* ctrl +e: 回到尾
	* ctrl+c:回答下一行
	
# 删除用户名和邮箱

# 从暂存区---》工作区
	* git rm --cached
	* git restore --statged 文件名
	
# 删除已提交的文件(已提交到本地仓库的文件)
	* git rm  文件名  (删除后，文件会回到 暂存区)

# 操作系统的删除
	* rm 文件名   (将文件放到 工作区)
	
# 执行以上的操作后
	* 在执行 git commit -m "彻底删除" 就彻底将文件删除
	
# 删除后怎么恢复(git rm 后悔)
	* 恢复到工厂区
		*  1. git reset head 文件名  (git restore --staged 文件民) 具体命令通过 git status 进行查看
		*  2. git checkout -- 文件名 (git restore  文件名)
# git status
	* 通过这个可以判断当前文件所处的 阶段
		*  eg:可以执行 add命令就还在工作区哦/commit命令 就还在 暂存区哦
		*  
# 文件重命名
	* 设计到 2个步骤：
		* 1.将原来的文件从原来的地方 删除 移动到另一个地方
		* 2.将移动后的文件进行重命名
		
	* git mv 文件名（文件重命名）

# 将重命名后的文件进行撤回
		
	*  git restore --staged  hello.txt

    *  git restore hello.txt
    
# 注释重写(重写提交说明)
	* git commit --amend -m '注释'
	
# 将不需要提交的文件不提交(文件的忽略)
	* 新建一个 .gitignore
	* 在 .gitignore  文件中配置要忽略的文件
		* eg:dir目录下的所有.txt文件  dir/**/*.txt
	* 空文件自动忽略
	
# 分支
	* 查看分支： git branch
	* 创建分支： git branch 分支名
	* 切换分支： git checkout 分支名
	* 删除分支： git branch -d 分支名  (在自己的分支下不能删除自己)
	* 创建分支并切换: git checkout -b 分支名
	细节： 在分支A中进行写操作，改操作在工作区(没有add,commit)那么在B分支可以看见改操作。否则看不见改操作。

	* 修改分支名：git branch -m 旧分支名  新分支名
	* 
# 查看所有的分支
	* git branch -v
	
# 分支
	* 一条commit链，记录了每次commit的记录
	* 分支名(master):当前最近的一次提交(有commit命令)
	* HEAD:指向当前的分支名(最新的一个分支名，即时没有commit)
	
# 分支合并
	* git merge 新的分支名

#如果一个分支靠前(eg:dev),一个分支落后(eg:master)。并且两个分支不冲突，可以通过merger，master就可以追赶dev分支了。称为 fast forward

# fast forward(本质时分支指针的移动)
	* 1.两个分支 fast forward后会归于同一个commit
	
# git 在合并(merge)时默认使用的时fast forward
	
# 如果两个分支 在 同一时刻进行合并，如果同时修改 某个文件，就会发生冲突。 如果俩个文件，不在  同一时刻，进行合并，不会发生冲突。并且落后的一方回去追赶 前面的分支。


 
# 查看所有的日志记录
	* git reflog
	
# 添加并提交
	* git commit -am '注释'  (改命令不能用在第一次)
	
	
# 可以在多个版本(commit)之间进行穿梭
	* 回退到上n次的commit: git reset --hard HEAD ~n
#


 
	
			