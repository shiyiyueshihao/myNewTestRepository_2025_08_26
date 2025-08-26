# myNewTestRepository_2025_08_26
学习git，学习如何将远程仓库与本地仓库进行连接并且进行一些简单的操作处理

# Git 本地添加远程仓库
# 创建远程仓库
  # 初始化本地仓库
    git init 
      
  # 为本地添加远程仓库
    git remote add <shortname> <url>
    shortname:远程仓库的简称，自定义； url:远程仓库的地址

      
    提示： 
      .git/config文件中可以查看远程仓库的信息
 
  # 查看远程仓库    
    git remote
      有两种方式 
      1. git remote
 <img width="867" height="195" alt="image" src="https://github.com/user-attachments/assets/899b6ed1-d865-48cc-ad9f-617acf568256" />
      
      2.打开初始化本地仓库地址的文件夹，然后找到.git 进入找到config  vscode打开即可
 <img width="843" height="351" alt="image" src="https://github.com/user-attachments/assets/c2cd4a2e-9848-4dbe-84c8-858a5aa76458" />

  # 删除远程仓库 
    git remote rm 仓库名
    提示： 
      此操作是本地移除与远程仓库的关联，并不是将远程仓库从平台上删除。
<img width="876" height="313" alt="image" src="https://github.com/user-attachments/assets/fb580ec1-c2ac-47f7-8b2a-b7ecd533bb52" />

  # 获取远程仓库代码
    git pull <远程主机名> <远程分支名>
<img width="1567" height="492" alt="image" src="https://github.com/user-attachments/assets/8ec754f9-08c8-4fbf-8a07-050798d2852d" />

  # 推送本地仓库代码到远程仓库
      git push <远程主机名> <本地分支名>:<远程分支名>
<img width="866" height="286" alt="image" src="https://github.com/user-attachments/assets/677e73e4-6eab-4b03-9914-7f38483d6fa2" />
(第一个问题出在  远程仓库修改了内容 而本地没有实时更新(git pull origin(myNewTest) main更新))
(第二个问题出现在网络部分)

    如果本地分支名与远程分支名相同，则可以省略冒号：
      git push <远程主机名> <本地分支名> 
      git push origin master
