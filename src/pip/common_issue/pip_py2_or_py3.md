# 使用pip时注意是Pyhton2还是Python3

在使用pip时，要注意`pip`的版本，是`Python 2`还是`Python 3`

可以通过：

```bash
pip --version
```

去确认当前pip到底是什么版本。

举例：

* Python 2
    ```bash
    ➜ pip --version
    pip 10.0.1 from /Users/crifan/Library/Python/2.7/lib/python/site-packages/pip (python 2.7)
    ```
* Python 3
    ```bash
    ➜ pip --version
    pip 10.0.1 from /usr/local/lib/python3.6/site-packages/pip (python 3.6)
    ```

在使用时，不要搞混了。

如果搞混了，容易出现问题：

用pip安装了库（到某个Python环境=python版本）中

但是去代码中（用到了另外一个环境=Python版本）去导入对应的库，却找不到该库，import会报错。
