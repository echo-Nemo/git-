#第一次进行项目--远程的关联
	* git remote add origin github中的ssh
	
#第一次发布项目（本地到远程）
	* git add .      //将本地文件 到 暂存区
	* git commit -m "注释内容"   //将暂存区 到 本地仓库
	* git push -u origin master
	
# 第一次从远程服务器上下载项目
	* git clone （点击项目中的clone下的ssh）
	
# 提交(第一次过后)(从本地到远程)
	* git add .
	* git commit -m ""
	* git push origin master
	
# 更新 （从远程到本地）
	* git pull
	
# 发生冲突
	* 服务器（远程仓库）和 本地分支 在修改同一个文件
	* 或者是2个人在修改同一个文件 
	# 解决方法
		* 一般使用merge 合并，然后再将本地的文件--》暂存区--》本地分支--》远程服务器

# 多人团队协作开发
	* github --->settin--->collaborators ---》加入合作者 github的全名---》发送邀请链接
	* 合作伙伴-——》打开改链接--》接受邀请---》项目clone--->修改-->add\commit\push
	* 