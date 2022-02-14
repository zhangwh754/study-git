## 创建并切换到新分支 dev

```
git switch -c dev
```

## 查看当前分支

```
git branch
```

`git branch`命令会列出所有分支，当前分支前面会标一个`*`号。

![image-20211109224541790](https://gitee.com/zhang754/blogimg/raw/master/img/image-20211109224541790.png)

## 正常提交

对 README 修改后提交

```
git add README.md
git commit -m "测试分支提交"
```

## 切换回原分支

```
git switch master
```

发现 dev 分支的修改的 README.md 内容全部消失了

## 合并内容

```
git merge dev
```

如果没有冲突此时 main 分支的 readme 文件将合并 dev 分支,两者一样

## 删除分支

```
git branch -d dev
```

## 冲突解决

新建分支并移动到分支 develop

```
git switch -c develop
```

在 develop 的 readme 添加冲突解决该段文字

在 develop 进行提交
不会影响 main 分支
main 分支添加任意文字，进行提交

![image-20211109232951666](https://gitee.com/zhang754/blogimg/raw/master/img/image-20211109232951666.png)

![image-20211109233013975](https://gitee.com/zhang754/blogimg/raw/master/img/image-20211109233013975.png)

![image-20211109233027077](https://gitee.com/zhang754/blogimg/raw/master/img/image-20211109233027077.png)

手动解决冲突再进行提交

再删除develop分支

```
git branch -d develop
```





## 查看历史提交修改的文件

```
git log --stat
```

![image-20211229154848978](https://gitee.com/zhang754/blogimg/raw/master/img/image-20211229154848978.png)

在 终端 按下q，可以离开git log



## 回退历史分支

```sh
git reset --hard 分支哈希值
```

