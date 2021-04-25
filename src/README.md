# 管理好Python的库：包管理器

* 最新版本：`v1.0`
* 更新时间：`20210425`

## 简介

介绍如何用包管理器尤其是pip去管理好Python的库。先进行基本的概述，包括常见的Python包管理器有easy_install、setuptools、pip；然后详细阐述pip：包括常用的命令，比如pip install、pip uninstall、pip show、pip list、pip search、pip freeze。其中包括pip install的各种语法和各种举例说明；以及如何给pip下载加速，包括更换源和加代理的方法和具体操作步骤；总结了pip常见的一些问题，包括command not found pip、Could not install packages due to an EnvironmentError Errno 13 Permission denied、Retrying after connection broken by NewConnectionError、使用pip时要注意是python2还是python3、以及部分可以情况下不用pip管理python的库；然后整理了pip相关的一些内容，包括虚拟环境工具pipenv、通过pip查看site-packages位置等；最后给出参考资料。

## 源码+浏览+下载

本书的各种源码、在线浏览地址、多种格式文件下载如下：

### Gitbook源码

* [crifan/python_summary_package_manager: 管理好Python的库：包管理器](https://github.com/crifan/python_summary_package_manager)

#### 如何使用此Gitbook源码去生成发布为电子书

详见：[crifan/gitbook_template: demo how to use crifan gitbook template and demo](https://github.com/crifan/gitbook_template)

### 在线浏览

* [管理好Python的库：包管理器 book.crifan.com](http://book.crifan.com/books/python_summary_package_manager/website)
* [管理好Python的库：包管理器 crifan.github.io](https://crifan.github.io/python_summary_package_manager/website)

### 离线下载阅读

* [管理好Python的库：包管理器 PDF](http://book.crifan.com/books/python_summary_package_manager/pdf/python_summary_package_manager.pdf)
* [管理好Python的库：包管理器 ePub](http://book.crifan.com/books/python_summary_package_manager/epub/python_summary_package_manager.epub)
* [管理好Python的库：包管理器 Mobi](http://book.crifan.com/books/python_summary_package_manager/mobi/python_summary_package_manager.mobi)

## 版权说明

此电子书教程的全部内容，如无特别说明，均为本人原创和整理。其中部分内容参考自网络，均已备注了出处。如有发现侵犯您版权，请通过邮箱联系我 `admin 艾特 crifan.com`，我会尽快删除。谢谢合作。

## 鸣谢

感谢我的老婆**陈雪**的包容理解和悉心照料，才使得我`crifan`有更多精力去专注技术专研和整理归纳出这些电子书和技术教程，特此鸣谢。

## 更多其他电子书

本人`crifan`还写了其他`100+`本电子书教程，感兴趣可移步至：

[crifan/crifan_ebook_readme: Crifan的电子书的使用说明](https://github.com/crifan/crifan_ebook_readme)
