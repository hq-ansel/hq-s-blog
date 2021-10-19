# 简单使用git!

### 1、创建本地仓库

```
git init
```

### 2、克隆仓库

```
#对于本地的仓库
git clone D:/myrepo
#对于服务器仓库
git clone username@host:/path
```

### 3、git工作流

![](https://rogerdudler.github.io/git-guide/img/trees.png)

### 4、添加和提交你的文件

```
#添加文件到暂存区
git add readme.md
#添加所有目录下文件
git add *
#提交更改到head
git commit -m"代码提交区"
```

### 5、把head的改动提交到远端

```
#提交到分支
git push origin branchname
#把现有仓库连接到远端
git remote add origin <server>
```

### 6、分支与合并

![](https://rogerdudler.github.io/git-guide/img/branches.png)

```
#创建分支
git checkout -b branchname
#切换分支
git checkout branchname
#把新建的分支删除
git branch -d branchname
#把分支发送到远端
git push origin branchname
```

### 7、更新与合并

```
#把本地仓库用远端更新
git pull
#把远端改动合并到当前分支
```

