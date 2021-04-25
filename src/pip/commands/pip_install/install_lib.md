# 用pip安装库

* 安装
  * 普通安装
  ```bash
  pip install xxx
  ```
    * 把pip作为python的模块去安装
      ```bash
      /your/specific/python -m pip install xxx
      ```
  * 安装特定版本
    ```bash
    pip install 'xxx==version_number'
    ```
  * 安装`A`时，同时安装A所依赖的库：`B`
    ```bash
    pip install A[B]
    ```
* 升级
  * 升级已安装的库
    ```bash
    pip install --upgrade xxx
    ```
    * 等价于
      ```bash
      pip install -U xxx
      ```

## 安装来源和方式

* 从文件安装
  * `whl文件`
    * `在线`文件
      ```bash
      pip install https://storage.googleapis.com/tensorflow/mac/cpu/tensorflow-1.7.0rc1-py3-none-any.whl
      ```
    * `本地`文件
      ```bash
      pip install /Users/crifan/dev/dev_tool/tensorflow/tensorflow-1.7.0rc1-py3-none-any.whl
      ```
* 从源安装
  * `源码包`
    * 语法
      ```bash
      pip install PackageName --no-index --find-links file:///path/to/your/package
      ```
    * 举例
      ```bash
      pip install -U SQLAlchemy --no-index --find-links ./SQLAlchemy-1.1.3.tar.gz
      ```

## `pip install`举例

* pipenv
  * 安装pinenv
    ```bash
    pip3 install pipenv --user
    ```
  * 用pip升级pipenv
    ```bash
    pip install --user --upgrade pipenv
    ```
* 安装Django的sendfile插件
  ```bash
  pip3 install django-sendfile
  ```
* 安装Django的CORS插件
  ```bash
  pip3 install django-cors-headers
  ```
* 安装查看文件类型的MIME
  ```bash
  pip install mime
  ```
* 安装Amazon的boto3
  ```bash
  pip install boto3
  ```
* 安装Web自动化工具`selenium`
  ```bash
  pip install -U selenium
  ```
* 安装虚拟环境工具`virtualenv`
  ```bash
  pip install virtualenv
  ```
  * 升级virtualenv
    ```bash
    pip install --upgrade virtualenv
    ```
* 安装MongoDB数据库的Python的driver
  ```bash
  pip install pymongo
  ```
  * 升级MongoDB
    ```bash
    pip install --upgrade pymongo
    ```
* 安装数据库ORM：sqlalchemy
  ```bash
  pip install -U sqlalchemy
  ```
  * 安装指定版本
    ```bash
    pip install 'sqlalchemy==1.1.0b3'
    ```
* 安装爬虫工具scrapy
  ```bash
  pip install scrapy
  ```

### 通过python的模块方式调用pip去安装

* 通过python的模块方式调用pip去安装pylint
  ```bash
  /usr/local/bin/python3 -m pip install -U pylint --user
  ```
  * 类似的写法
    ```bash
    python -m pip install -U pylint
    ```

### 安装之前加额外参数

* 在重新安装pycurl之前，加上额外的参数
  ```bash
  pip uninstall pycurl
  export PYCURL_SSL_LIBRARY=openssl
  export LDFLAGS=-L/usr/local/opt/openssl/lib;export CPPFLAGS=-I/usr/local/opt/openssl/include;pip install pycurl --compile --no-cache-dir
  ```


### 安装库A同时安装依赖库B

* 安装gunicorn同时安装所依赖的其他库
  * eventlet
    ```bash
    pip install gunicorn[eventlet]
    ```
  * gevent
    ```bash
    pip install gunicorn[gevent]
    ```
  * tornado
    ```bash
    pip install gunicorn[tornado]
    ```
  * gthread
    ```bash
    pip install gunicorn[gthread]
    ```

### 给出部分库的详细安装日志

* 安装Python项目部署工具supervisor
  ```bash
  pip install supervisor
  ```
  * 如果遇到权限问题，则加上`--user`
    ```bash
    pip install supervisor --user
    ```
      * 详细日志
        ```bash
        ➜  robotDemo pip install supervisor --user
        Collecting supervisor
        Collecting meld3&gt;=0.6.5 (from supervisor)
          Using cached https://files.pythonhosted.org/packages/b6/ae/e6d731e4b9661642c1b20591d8054855bb5b8281cbfa18f561c2edd783f7/meld3-1.0.2-py2.py3-none-any.whl
        pipenv 11.10.0 requires certifi, which is not installed.
        pipenv 11.10.0 requires requests[security], which is not installed.
        pipenv 11.10.0 requires virtualenv, which is not installed.
        matplotlib 1.3.1 requires nose, which is not installed.
        matplotlib 1.3.1 requires tornado, which is not installed.
        Installing collected packages: meld3, supervisor
          The scripts echo_supervisord_conf, pidproxy, supervisorctl and supervisord are installed in '/Users/crifan/Library/Python/2.7/bin' which is not on PATH.
          Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.
        Successfully installed meld3-1.0.2 supervisor-3.3.4
        ```
* 安装Excel处理工具`openpyxl`
  ```bash
  pip install openpyxl
  ```
  * 详细日志
    ```bash
    ➜  英语资源 pip install openpyxl
    Collecting openpyxl
      Downloading openpyxl-2.5.1.tar.gz (169kB)
        100% |████████████████████████████████| 174kB 1.1MB/s
    Collecting jdcal (from openpyxl)
      Downloading jdcal-1.3.tar.gz
    Collecting et_xmlfile (from openpyxl)
      Downloading et_xmlfile-1.0.1.tar.gz
    Building wheels for collected packages: openpyxl, jdcal, et-xmlfile
      Running setup.py bdist_wheel for openpyxl … done
      Stored in directory: /Users/crifan/Library/Caches/pip/wheels/98/5e/20/70cde417026f1e168acdac7babf47b204a7b752b1a8e6bb795
      Running setup.py bdist_wheel for jdcal … done
      Stored in directory: /Users/crifan/Library/Caches/pip/wheels/0f/63/92/19ac65ed64189de4d662f269d39dd08a887258842ad2f29549
      Running setup.py bdist_wheel for et-xmlfile … done
      Stored in directory: /Users/crifan/Library/Caches/pip/wheels/99/f6/53/5e18f3ff4ce36c990fa90ebdf2b80cd9b44dc461f750a1a77c
    Successfully built openpyxl jdcal et-xmlfile
    Installing collected packages: jdcal, et-xmlfile, openpyxl
    Successfully installed et-xmlfile-1.0.1 jdcal-1.3 openpyxl-2.5.1
    ```
