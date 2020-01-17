---
title: "Tuesday Week1"
date: 2020-01-14
description: "What is Git"
tags: [Git]
---



Today I learned what is [Git][] and how does it work.  

>Git is a kind of **version-control system (VCS)**, which is a program that tracks changes to a collection of files. One goal is to easily recall earlier versions of individual files or the entire project. Another is to allow several team members to work on a project, even on the same files, at the same time without impacting each other. And Git is a **fast, versatile, highly scalable, free, open-source** version-control system.   

Firstly, I need to figure out some **terminologies**  about the Git  

* Working tree: The set of nested directories and files that contain the project being worked on.  
* Repository (repo): The directory, located at the top level of a working tree, where Git keeps all of the history and metadata for a project.   
* Hash: A number produced by a hash function that represents the contents of a file or other object to a fixed number of digits. Git can tell whether a file has changed by hashing its contents and comparing the result to the previous hash.   
* Commit: It means you are committing the changes you have made so others can eventually see them, too.  
* Branch: A named series of linked commits. The most recent commit on a branch is called the *head*. The default branch, which is created when you initialize a repository, is called "*master*."  

Next, I learned several simple commands of Git and tried to use them in a sandbox.   

1. To double check that Git is installed, use  
        
        git --version  
    You should see output that looks something like  

        git version 2.7.4  
2. To configure Git, you must define some global variables: `user.name` and `user.email`. Both are required for commits.  

        git config --global user.name "<USER_NAME>"  
        git config --global user.email "<USER_EMAIL>"  
    And you can use  
        
        git config --list  
    to confirm your configuration.  
3. Create a folder named "test". This folder will be the working tree (sometimes called a "project directory") where your Web site is stored and the files that comprise it are located.  

        mkdir test
    To change the directory, use `cd` like

        cd test  
4. Then execute a `git init` command to initialize the repository.  

    To show the  status of the working tree, use

        git status  
5. Use an `ls` command to show the contents of the working tree  

        ls -a  
6. To get help with what you can do with Git, type  

        git --help  
7. You will use   

        git add   
    to *stage* changes to prepare for a commit. All changes in files that have been added, but not committed yet are stored in the *staging area*.  
    You can also use  

        git add .    
    to add all the files in a directory.  
8. Once you've *staged* some changes for commit, you can save your work into a snapshot by invoking the command  

        git commit  
9. You can use  
        
        git log  
    to see information about previous commits.  
10. You can use `touch` command to update a file's last-modified time if the file exists, or create an empty file if it does not.  
11. Open the online editor by typing a `code` command.  
12. Use a `git diff` command to see what changed.  
13. Delete a file by `rm` command.  

It looks **good**! All of the commands are working properly.  



****************************  



今天，我了解了什么是[Git][]，以及它是如何工作的。  

>Git是一种**版本控制系统（VCS）**，是一个跟踪文件集内更改的程序。它的一个目的是轻松调用单个文件或整个项目的早期版本。另一个是允许多个团队成员同时处理一个项目，即使是同时处理相同的文件，也不会互相影响。Git是一个**快速、通用、高度可扩展、免费、开源的**版本控制系统。  

首先，我需要搞清楚有关Git的一些术语

* 工作树：包含正在处理的项目的一组嵌套目录和文件。  
* 版本库（repo）：该目录位于工作树的顶层，Git在此保留了项目的所有历史记录和元数据。  
* 哈希：由哈希函数产生的数字，它将文件或其他对象的内容表述为固定位数的数字。Git可以通过对文件内容进行哈希处理并将其结果与​​先前的哈希数进行比较来判断文件是否已被更改。  
* 提交：即您正在提交所做的更改，以便其他人最终也可以看到它们。  
* 分支：一系列命名的关联提交。对分支的最新提交称为*head*。初始化版本库时创建的默认分支称为“*master*”。  

接下来，我学习了一些简单的Git命令，并尝试在沙箱中使用它们。  

1. 检查Git已经安装完成，输入  

        git --version  
    应该看到类似以下的输出  

        git version 2.7.4  
2. 要配置Git，必须定义一些全局变量：`user.name`和`user.email`。两者都是完成提交这一指令所必需的。  

        git config --global user.name "<USER_NAME>"  
        git config --global user.email "<USER_EMAIL>"    
    可以用  

        git config --list  
    来确认配置。  

3. 创建一个名为“test”的文件夹。该文件夹会成为工作树（有时称为“项目目录”），网站以及它所包含的的文件都在这里。  

        mkdir test
    要更改目录，使用`cd`，比如  

        cd test  
4. 执行`git init`命令来初始化存储库  

        git init  
    
    要显示工作树的状态，使用  

        git status  
5. 使用ls命令显示工作树的内容  

        ls -a  
6. 要获得有关Git功能的帮助，输入  

        git --help   
7. 使用  

        git add    
    *暂存*更改来为提交做准备。所有已被添加但尚未被提交的文件中的更改都将存储在*暂存区*中。  
    
    也可以使用  

        git add .    
    将所有文件添加到目录中。  

8. 一旦更改被*暂存*并准备被提交，就可以使用如下指令来将工作保存在快照中。  

        git commit  
9. 使用  

        git log  
    查看有关先前提交的信息。  

10. 使用`touch`指令来更新文件的上次修改时间（如果文件存在），或者创建一个空文件（如果不存在）。  

11. 通过键入`code`命令来打开在线编辑器。  

12. 使用`git diff`命令来查看更改。  

13. 通过`rm`命令来删除文件。  

看起来不错！所有命令都能正常运行。



[Git]: https://git-scm.com/