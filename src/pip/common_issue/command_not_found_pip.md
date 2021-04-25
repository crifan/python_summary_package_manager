# command not found pip

**现象**：用pip去安装`virtualenv`期间出错：

```bash
~ pip
zsh: command not found: pip
```

**原因**：当前CentOS服务器中没有安装pip

**解决办法**：去CentOS中安装pip

**操作步骤**：

先用`yum`安装`python-pip`：

```bash
yum -y install python-pip
```

再去升级到最新版：

```bash
pip install --upgrade pip
```

即可