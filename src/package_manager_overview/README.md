# Python包管理器概述

Python开发期间，经常涉及到需要安装各种Python库，用于实现不同的功能。

Python中用**包管理器**来管理Python库。

目前现存有很多种Python的包管理器：

* Python包管理器
  * `easy_install`
      * `easy_install`基于旧的包格式：`egg`
      * 现在很少用了
        * 只有当你只有`egg`的格式时，才需要用到`easy_install`
  * `setuptools`
    * `setuptools`包含了（内部用到了）`easy_install`
    * 现在用的很少
  * **<font color=red>pip</font>**
    * 历史
      * 2008年发布
    * 内部实现
      * 基于新的包的格式：`wheel`
    * `pip`往往是Python自带就有的，无需额外安装。且功能强大，很好用。
    * `pip`是目前Python中**最常见**的包管理器
