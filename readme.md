github使用教程
===

1.版本控制器：
---
    git和svn的区别：
	svn：集中式
	git：分布式

2.识别用户名和密码：
---
<code>
	$ git config --global user.name "Your Name"
	$ git config --global user.email "email@example.com"
</code>

3.通过 <code> git init </code>命令把当前的目录变成一个仓库
---

注意：dir修改为ls  使用<code> ls -ah </code>可以查看隐藏文件

4.版本库添加文件：
---
   <code> git add filename </code>
5.版本库提交文件
---
   <code> git commit -m ‘备注’ </code>
6.查看版本库状态：
---
   <code> git status </code>
7.查看文件的修改： 需要文件没有被添加和提交才可以查看
---
   <code> git diff </code>
8.查看历史版本
---
   <code> git log  </code>
   简化输出信息：<code> git log --pretty=oneline </code>
9.回退或回到某个版本
---
   <code> git reset --hard HEAD^ (版本代码) </code>

10.工作区和暂存区：
---
    工作区：当前正在编写代码的区域
    暂存区：通过git add提交的区域

11.管理修改：
---
    如果遇到刚刚所述问题：
        1.每次修改完记得add
        2.不管什么时候，全部add在提交

12.撤销修改：
---
     <code> git checkout -- filename </code>

13.创建与合并分支：
---
    查看分支：<code> git branch </code>
    创建分支：<code> git branch <name> </code>
    切换分支：<code> git checkout <name> </code>
    创建+切换分支：<code> git checkout -b <name> </code>
    合并某分支到当前分支：<code> git merge <name> </code>
    删除分支：<code> git branch -d <name> </code>

14.冲突：手动修改文件
---


15.关联github：
---
    1.关联<code> github：git remote add origin git@github.com:Geekiwen/hello.git </code>
    2.将本地版本库推送到服务器上：<code> git push -u origin master </code>