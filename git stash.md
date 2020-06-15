# stash:保存现场
	* 1.(建议 规范):在功能没有开发完成时，不要commit
	* 2. 规定：在没有commit之前不要checkout切换分支(两个分支不再同一个commit阶段)
	* 如果某一个功能还没有开发完毕，就要切换分支
		* 建议： 1. 保存现场（临时保存，git stash,相当于有个备份
# 保存现场
	* git stash
	
# 查看现场
	* git stash list
	
# 还原现场(默认只还原最近的一次)结构是一个栈
	* git stash pop （将原来保存的删除，用于还原内容）
	* git stash apply (还原内容，还原之后不会删除原来保存的内容),
	* 指定某个特定的现场： git stash apply 现场的名字
# 手动删除现场
	* git stash drop 现场的名字
	
# Tag标签：适用于整个项目，和具体的分支没有关系
	* 给标签取名： git tag xxxx
	* 查看标签: git tag
	* 模糊查询标签的名字： git tag -l 'v2*'  (eg:以v2开头的所有标签)
	* 删除标签 git tag -d  标签名
	
# 责任
	*  git blame a.txt  查看a.txt的所有提交的commit记录

# 查看 暂存区和工作区的差异
	* git diff

# 查看 分支区 和 工作区的差异
	* git diff commit sha值(git log中的值)
# 查看 最新的 分支区 和 工作区的差异
	* git diff commit HEAD

# 查看 分支区和 暂存区的差异
	* git diff --cached commit的sha1值
# 查看最新的 分支区和暂存区 区别
	* git diff --cached HEAD
	
# 各种分支的区别
	* dev:开发分支，可以频繁的改变
	* test: 基本开发完毕后，交给测试实施人员
	* master: 生产阶段，一般很少改变
	* 

# git remote show 
	* 查看远程的分支
# git会在本地维护 origin/master分支，通过改分支，可以感知远程github的内容，origin/master 一般建议 不要修改，只是一个只读分支


# push/pull :推送，会改变指针

# Fast-forward: 更新，

#又冲突
	* 进行pull=fetch+merge
	* 将冲突merger解决后 -->在从新 add/commit/push
	* 
	*
