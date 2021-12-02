# 创建SSHKey

**创建SSHKey：**
```bash
ssh-keygen -t rsa -C "your_email@example.com"
```
**查看Key内容：**
```bash
cat ~/.ssh/id_rsa.pub
```
**问题一：**

<p class="warn">Permissions 0644 for '/root/.ssh/id_rsa.pub' are too open</p>

执行以下命令：
```bash
chmod 0600 ~/.ssh/id_rsa
cat ~/.ssh/id_rsa.pub
```
