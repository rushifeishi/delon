* 首先要先确定一下是否建立了主repo的远程源：

   ` git remote -v`

* 如果里面只能看到你自己的两个源(fetch 和 push)，那就需要添加主repo的源：
```
git remote add upstream https://github.com/ng-alain/delon.git
git remote -v
```
然后你就能看到upstream了。
* 如果想与主repo合并：
```
git fetch upstream
git merge upstream/master
```