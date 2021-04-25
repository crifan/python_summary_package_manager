# pip freeze

## 用`pip freeze` + `pip install`备份和恢复Python环境

pip的常见用法之一包括：

在别处，用pip给某项目安装了相应的库之后，去`freeze`=`冻结`：

```bash
pip freeze > requirements.txt
```

即，把当前Python中安装的所有的库的信息，写入到一个文本文件中。

该文件文件常写成`requirements.txt`，表示当前Python环境**所需**的库的信息。

而换到另外一个地方，想要恢复之前项目的环境，则可以用：

```bash
pip install -r requirements.txt
```

即可自动安装所依赖的，各种Python的库，恢复了之前的项目的Python环境。


