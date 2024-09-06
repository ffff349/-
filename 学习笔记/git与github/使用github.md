
- 在线创建一个自己的库
	- ![[Pasted image 20240906134936.png]]
	- ![[Pasted image 20240906134952.png]]
- ### **Git 和 GitHub 的绑定**
	- 获取SSH keys  输入 cd ~/.ssh，返回"no such file or directory"表明电脑没有ssh key，需要创建ssh key。
	- ssh-keygen -t rsa -C “git账号”
		- 例如 ： ssh-keygen -t rsa -C “1724177606@qq.com”
		- 输入之后一路（三次）Enter（确认）就可以了
		- 一下截图就说明成功了
			- ![[Pasted image 20240906135254.png]]
		- 接着打开id_rsa.pub文件，复制里面的内容。
	- 接下来我们需要登录到我们的GitHub上边添加这个密匙
		- ![[Pasted image 20240906135426.png]]
		- ![[Pasted image 20240906135433.png]]
	- 在终端输入：ssh -T git@github.com
		- ![[Pasted image 20240906135624.png]]
		- 如果输入代码之后再选择yes出来是这样说明就成功啦！！！
	- 接下来设置全局信息，这两个的顺序可以颠倒，没有固定的顺序。
		- git config --global user.name “gitname”  
		- git config --global user.email “git邮箱”


- push 和 pull 
	- 复制git链接
	- 使用 git clone 
		- ![[Pasted image 20240906140336.png]]
		
git add ./
git commit -m "备注"
git push origin main

git pull origin main

参考链接：
	https://chunqiushenye.blog.csdn.net/article/details/140707647?spm=1001.2014.3001.5502
	https://blog.csdn.net/m0_57787115/article/details/130296388