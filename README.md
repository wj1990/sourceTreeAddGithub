
sourceTree添加github ssh
=====
1.安装git 然后配置本地 github账户 
-----
	$ git config --global user.name "xxx" ---回车
	$ git config --global user.email "xxx.mail@xxx.com"   ---回车
2.使用 git 客户的生成公私钥
-----
	$ ssh-keygen -t rsa -C "xxx.mail@xxx.com"
	连续3个回车，密码为空  
	会在计算机生成  id_rsa id_rsa.pub 两个文件 公钥 私钥
3.sourceTree设置 ssh
-----
	点击-->>工具-->>选项   找到 ssh客户端 ：设置openSSH  ---确定
4.添加 本地~/.ssh/id_rsa.pub 公钥到github
-----
	打开github-->>设置 -->>ssh  
	新建 title随意 将本地 id_rsa.pub内容复制到 key里面  ----确定 完事
	
注意事项：
----
	由于我刚用sourcetree拉取代码 用的是 https方式 
	https://github.com/wj1990/sourceTreeAddGithub.git
	所以刚提交了一次 还需要输入用户名密码
	应该用 ssh git@github.com:wj1990/sourceTreeAddGithub.git

测试一下 我在这个地方做了修改
----