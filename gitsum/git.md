# git

##### 1,什么是版本控制和版本控制的发展

​	

##### 2.安装git 和 文件的三个状态三个存放空间

​	文件有 modify 暂存 和 提交 三种状态

​	对应 三个空间 工作空间，暂存空间 ，和git仓库

​	git add 文件

​	git commit  -m "注解" 

##### 3.文件的修改 和 比对 

​	修改已经提交的文件， 是文件处于 modify 需要 add 暂存区 然后 commit 提交

​    比对  git diff HEAD -- 文件名 

​	head ，指向的是目前新的版本 

##### 4.版本切换

 每个版本由唯一标识的 哈希序列

 通过 git reset -hard HEAD^	 来回退到上一个 通过^^ 是上上一个 

 也可以通过 git reset --hard Head~num 来回退 上num个

版本向前后  通过 git reset --hard 版本序列（只需要前7个就行）

##### 5.文件删除

工作空间内文件删除后恢复  

​		git checkout 文件名+后缀

本地git仓库删除文件

​		git rm 文件名 + 后缀 （删除后不易找回）