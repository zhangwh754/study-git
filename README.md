## 创建并切换到新分支dev

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

对README修改后提交

```
git add README.md
git commit -m "测试分支提交"
```

## 切换回原分支

```
git switch master
```

