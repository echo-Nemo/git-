# git命令（分布式版本控制）
	# 每个人 都有一个本地版本库（分支）
		*  
	* git add:将本地文件 增加到暂存区
	* git commit:将暂存区的内容 提交到 本地仓库(仓库分支)
	* git push:将本地仓库的内容 推送到 远程仓库（远程分支）
	* git pull:将远程仓库(远程分支)中的内容 拉取到本地仓库（本地分支）
	
# 配置 git的用户名和密码
	* git config --global user.name "用户名"
	* git config --global user.email "邮箱"
	* 配置成功后就会在本地看到一个.gitconfig的文件
# git的服务器:统一的托管网站 github

# 为了在本地 和远程仓库之间 进行免密钥的登入，通过ssh进行登入
	* ssh-keygen -t rsa -C 邮箱名
	* 一直回车,在本地的指定的盘中就会有一个密钥
	
# 将本地的密钥给远程服务器
	* setting---:ssh and ....-> key中输入 id_ras.pub中的内容，不要有回车符
	
# 测试是否连通成功
	* ssh -T git@github.com    在本地目录中有个know_host的文件
	
# 在本地新增git项目，发送到远程
	* 进入项目的文件夹 --> 右键git bush 
	* git init
	* 
# 远程创建一个项目
	* 会有一个标识hhtp/ssh
	
# 将本地项目和远程项目进行关联
   * git remote add origin git@github.com:echo-Nemo/gitproject.git