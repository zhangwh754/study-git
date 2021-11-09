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

发现dev分支的修改的README.md内容全部消失了

## 合并内容

```
git merge dev
```

如果没有冲突此时main分支的readme文件将合并dev分支,两者一样

## 删除分支

```
git branch -d dev
```

main分支添加任意文字，进行提交
