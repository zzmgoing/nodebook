# 安装配置git

**安装git：**
```bash
brew install git
```
安装路径：/usr/local/Cellar/git/

**查看git用户信息：**
```bash
git config user.name
git config user.email
```
**配置git用户信息：**
```bash
git config --global user.name "username"
git config --global user.email "your_email@example.com"
```
**更新git用户信息：**
```bash
git config --replace-all user.name "username"
git config --replace-all user.email "your_email@example.com"
```

**局部配置git用户信息：**

命令去掉--global，且局部配置需要到需要配置的git项目中进行配置，且局部配置将会覆盖全局变量。
