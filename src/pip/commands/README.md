# pip常用命令

pip常用的命令有：

* `pip install`
* `pip uninstall`
* `pip search`
* `pip show`
* `pip list`
* `pip freeze`

后续会详细介绍。

## 典型的pip使用逻辑

对于使用pip管理Python库的典型逻辑是：

用`virtualevn`或`pipenv`等创建某Python项目的Python虚拟环境后

进入虚拟环境，然后

* 去用`pip install xxx`安装需要用到的库

Python项目开发期间：

* 如果不需要某库，用`pip uninstall xxx`去删除掉
* 如果不知道某个库的包名是什么，但知道库的名字，可以用`pip search xxx`去找找源中是否有该库，以及具体包名是啥
* 想要知道具体某个已安装的库的详情（比如版本，具体安装位置等），可以用`pip show xxx`去查看
* 查看当前都安装了哪些库，用`pip list`

项目开发完毕后，`冻结`环境，即保存好当前Python环境，用：

```bash
pip freeze > requirements.txt
```

即生成了`requirements.txt`，记录了当前安装了哪些Python库，及其版本信息。

如果别人（比如你的同事接手你的项目）想要重新恢复你的Python项目的环境，则去：

（用和你一样的`virtualenv`或`pipenv`）创建对应的虚拟环境后，进入虚拟环境，再去：

```bash
pip install -r requirements.txt
```

安装全部的库，即恢复出了相同的Python环境。

即可，接着愉快的继续（协作）开发项目了。

## pip语法

`pip`的语法，可以通过help查看到：

```bash
pip --help
```

贴出来供参考：

```bash
 ⚙ limao@xxx  ~  pip --help

Usage:
  pip <command> [options]

Commands:
  install                     Install packages.
  download                    Download packages.
  uninstall                   Uninstall packages.
  freeze                      Output installed packages in requirements format.
  list                        List installed packages.
  show                        Show information about installed packages.
  check                       Verify installed packages have compatible dependencies.
  config                      Manage local and global configuration.
  search                      Search PyPI for packages.
  cache                       Inspect and manage pip's wheel cache.
  wheel                       Build wheels from your requirements.
  hash                        Compute hashes of package archives.
  completion                  A helper command used for command completion.
  debug                       Show information useful for debugging.
  help                        Show help for commands.

General Options:
  -h, --help                  Show help.
  --isolated                  Run pip in an isolated mode, ignoring environment variables and user configuration.
  -v, --verbose               Give more output. Option is additive, and can be used up to 3 times.
  -V, --version               Show version and exit.
  -q, --quiet                 Give less output. Option is additive, and can be used up to 3 times (corresponding to WARNING,
                              ERROR, and CRITICAL logging levels).
  --log <path>                Path to a verbose appending log.
  --no-input                  Disable prompting for input.
  --proxy <proxy>             Specify a proxy in the form [user:passwd@]proxy.server:port.
  --retries <retries>         Maximum number of retries each connection should attempt (default 5 times).
  --timeout <sec>             Set the socket timeout (default 15 seconds).
  --exists-action <action>    Default action when a path already exists: (s)witch, (i)gnore, (w)ipe, (b)ackup, (a)bort.
  --trusted-host <hostname>   Mark this host or host:port pair as trusted, even though it does not have valid or any HTTPS.
  --cert <path>               Path to alternate CA bundle.
  --client-cert <path>        Path to SSL client certificate, a single file containing the private key and the certificate in
                              PEM format.
  --cache-dir <dir>           Store the cache data in <dir>.
  --no-cache-dir              Disable the cache.
  --disable-pip-version-check
                              Don't periodically check PyPI to determine whether a new version of pip is available for
                              download. Implied with --no-index.
  --no-color                  Suppress colored output.
  --no-python-version-warning
                              Silence deprecation warnings for upcoming unsupported Pythons.
  --use-feature <feature>     Enable new functionality, that may be backward incompatible.
  --use-deprecated <feature>  Enable deprecated functionality, that will be removed in the future.
```
