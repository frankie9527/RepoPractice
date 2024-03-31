# 描述

## 当前仓库是一个repo 仓库，执行如下命令，便可拉下repo 仓库

```
repo init -u https://github.com/frankie9527/RepoPractice  -b main -m default.xml
repo sync
```
## xml 书写方式
```
<manifest>
    fetch ：远端的baseUrl
    <remote name="github" fetch="https://github.com/frankie9527" />
    revision ：这个指的是分支
    <default revision="main" remote="github" />
    //下面代码指的是 从 https://github.com/frankie9527/ArchitecturePractice 的mvvm 分支下代码到App/ArchitecturePractice
    //文件夹
     <project path="App/ArchitecturePractice" name="ArchitecturePractice" revision="mvvm"/>
</manifest>
```

如果不懂怎么写xml也可以参照一下[meta-riscv](https://github.com/riscv/meta-riscv)

## [repo 环境搭建](https://frankie9527.github.io/posts/git-repo/)