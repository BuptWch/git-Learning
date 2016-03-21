# git-Learning-1
学习使用git

1.1 git 命令行

    $ git  不带任何参数的列出git的选项和最常用的子命令
    
    $ git help --all  得到完整的git子命令列表
    
    $ git help subcommand  可查看每个git子命令的文档，如git help commit

1.2 git使用快速入门

  1.2.1 创建初始版本库 
  
  首先使用cd命令到工作目录，然后输入命令 
  
    $ git init 
  
  	git不关心是从完全空白的目录还是装满文件的目录开始，其将目录转换到git版本库的过程是一样的。
  	git init 命令创建一个新的版本库，最初每个版本库都是空的。为了管理内容，必须明确的把它放到版本库中。

1.2.2 将文件添加到版本库中

	  使用命令git add file将file 添加到版本库中 如 git add index.html
	  
	  如果目录中已经有了很多文件，使用 	$ git add.  命令把当前目录及子目录中的文件都添加到版本库
	
		add只是暂存了该文件，这是提交之前的中间步骤。git将add和commit分开，以避免频繁变化。
	
		$ git status  显示工作树状态
		
1.2.3 配置提交作者

	$ git config --global user.name "Firstname Lastname"
	$ git config --global user.email "your_email@example.com"
	
1.2.4 提交

	$ git commit -m "这里填上提取的日志"   add 之后 commit
	
	$ git commit filename -m "提取日志"  修改过后重新提交，无须add,之前已添加
	
1.2.5 查看提交

	$ git log  该命令会产生版本库里一系列单独提交的历史
	
	$ git show 提交码   查看提交的更详细信息，若没有指定提交码，显示最近一次提交信息
	
	$ git show-branch --more=10    提供当前开发分支简洁的单行摘要，"--more=10"表示额外10个版本
	
1.2.6 查看提交差异

	$ git diff 提交码1 \ 提交码2
	
1.2.7 版本内文件删除与重命名

	删除文件
	
		$ rm filename
		
		$ git commit -m "remove the file"
		
	重命名
	
		$ mv filename filename
		
1.2.8 创建版本库副本

	$ git clone projectname1 projectname2
	
	
	








