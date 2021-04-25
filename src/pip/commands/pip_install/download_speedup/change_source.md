# 更换pip的源

## 思路

* 新建（全局的、系统的）`pip`的配置文件
  * `Windows`：`%HOMEPATH%\pip\pip.ini`
    * 举例
      * `C:\Users\Administrator\pip\pip.ini`
  * `macOS`：`~/.pip/pip.conf`
    * 举例
      * `/Users/crifanli/.pip/pip.conf`
* 给配置文件加上国内的某个pip的源

## 步骤

（如果不存在的话）新建pip的配置文件

```bash
mkdir ~/.pip
vim ~/.pip/pip.conf
```

去更新配置内容，格式是：

```ini
[global]
index-url = pypi_mirror_url

[install]
trusted-host=pypi_mirror_url_host
```

参数解释：

* pypi_mirror_url
  * 常见可选的pip的源
    * 阿里云：http://mirrors.aliyun.com/pypi/simple/
    * 清华大学：https://pypi.tuna.tsinghua.edu.cn/simple
    * 豆瓣：http://pypi.douban.com/simple
* pypi_mirror_url_host
  * 对应`host`
    * `mirrors.aliyun.com`
    * `pypi.tuna.tsinghua.edu.cn`
    * `pypi.douban.com`

下面给出实例：

### 推荐：清华大学的pip的源

```ini
[global]
index-url = https://pypi.tuna.tsinghua.edu.cn/simple

[install]
trusted-host=pypi.tuna.tsinghua.edu.cn
```

实测：速度暴快，>`1MB/s`

### 推荐：阿里云的pip的源

```ini
[global]
index-url = http://mirrors.aliyun.com/pypi/simple

[install]
trusted-host=mirrors.aliyun.com
```

速度也不错，也很稳定。

### 可选：豆瓣的pip的源

```ini
[global]
index-url = http://pypi.douban.com/simple

[install]
trusted-host=pypi.douban.com
```

### 待确认：淘宝taobao的源

后来看到淘宝的npm的镜像

[taobao Mirrors](https://npm.taobao.org/mirrors/)

其中也能找到python的源：

[Python Mirror](https://npm.taobao.org/mirrors/python/)

抽空试试是否可用

### 特殊：现已不推荐：ustc的源

之前推荐的

```ini
[global]
index-url = http://pypi.mirrors.ustc.edu.cn/simple

[install]
trusted-host=pypi.mirrors.ustc.edu.cn
```

现已不推荐

原因：

* 其内部已跳转到tsinghua的源
  * 202104 后记：现已跳转到 BFSU（北京外国语大学）的镜像了：mirrors.bfsu.edu.cn
