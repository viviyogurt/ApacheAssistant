# ApacheAssistant
software experiment of buaa

## 项目git管理说明

+ 初次参与

本项目目前采用git进行管理，参与者初次使用

    git clone  https://github.com/buaa0110/ApacheAssistant.git

命令克隆本项目至本地开发环境

+ 提交

当开发者需要提交新的修改时，应依次使用以下命令

    git add .
    git commit -m "提交信息"
    git push

+ 合并修改

当开发者本地进行了修改而尚未确定origin是否有修改或者确定origin已存在修改时，请使用

    git stash
    git pull
    git stash pop

命令将本地修改与origin变化合并后在进行提交

- 比较本地和远程分支的差异

```
#比较本地和远程分支相差的commit
git fetch origin
git log master..origin/master

#比较本地和远程分支文件内容的改动
git fetch origin
git diff --stat master origin/master	#查看所有文件各修改了多少行
git diff master origin/master			#查看所有文件的具体内容改动
git diff master origin/master README.md	#查看某个文件的具体内容改动
```

