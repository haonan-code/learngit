# :smile:git使用：

1、在master分支上branch出dev分支

2、pull远端最新代码，然后在dev分支上进行开发

3、提交dev分支的代码（add--->commit--->push）

4、切换到master分支进行merge，如有冲突就解决后合并

5、再切回dev分支进行开发

## :zap:您总结的 Git 使用流程看起来是一个基本的工作流程，但还有一些需要注意的细节。以下是更详细的步骤：

在 master 分支上创建并切换到 dev 分支：

```
git checkout -b dev
```

拉取远程仓库的最新代码：

```
git pull origin master
```

在 dev 分支上进行开发，并添加、提交和推送更改：

```
git add .

git commit -m "commit message"

git push origin dev
```

切换回 master 分支并将 dev 分支合并到 master 分支：

```
git checkout master

git merge dev
```

如果存在冲突，则解决冲突并重新提交更改。如果没有冲突，则可以直接推送合并后的更改：

```
git push origin master
```

切换回 dev 分支并继续开发：

```
git checkout dev
```

需要注意的是，在步骤 4 中，如果存在与 dev 分支不兼容的更改，则可能会出现合并冲突。在这种情况下，您需要手动解决冲突并重新提交更改。另外，请确保在推送任何更改之前进行适当的代码审查。
