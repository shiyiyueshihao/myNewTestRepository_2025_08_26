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
 
  # 删除远程仓库 
    git remote rm 仓库名
    提示： 
      此操作是本地移除与远程仓库的关联，并不是将远程仓库从平台上删除。
    
  # 获取远程仓库代码
    git pull <远程主机名> <远程分支名>
    
  # 推送本地仓库代码到远程仓库
      git push <远程主机名> <本地分支名>:<远程分支名>
    
    如果本地分支名与远程分支名相同，则可以省略冒号：
      git push <远程主机名> <本地分支名> 
      git push origin master
