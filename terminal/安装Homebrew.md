# 安装Homebrew

[mac下高效安装 homebrew 及完美避坑姿势 （亲测有效）](https://www.cnblogs.com/joyce33/p/13376752.html)

**执行以下命令：**
```bash
/bin/bash -c "$(curl -fsSL https://cdn.jsdelivr.net/gh/ineo6/homebrew-install/install.sh)"
```
**更新镜像源：**
```bash
git -C "$(brew --repo)" remote set-url origin https://mirrors.ustc.edu.cn/brew.git
```
```bash
git -C "$(brew --repo homebrew/core)" remote set-url origin https://mirrors.ustc.edu.cn/homebrew-core.git
```
```bash
brew update
```

**问题一：**

<a href="https://www.jianshu.com/p/0353667c8f72">解决Mac安装Homebrew时‘Permission denied’问题</a>

执行以下命令：
```bash
sudo chgrp -R admin /usr/local
sudo chmod -R g+w /usr/local
```