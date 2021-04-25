# 通过pip查看site-packages位置

有时候，希望知道当前Python的`site-packages`的位置。

此时可以借用`pip show xxx`去实现。

举例：

```bash
# pip3 show Django
Name: Django
Version: 2.0.6
Summary: A high-level Python Web framework that encourages rapid development and clean, pragmatic design.
Home-page: https://www.djangoproject.com/
Author: Django Software Foundation
Author-email: foundation@djangoproject.com
License: BSD
Location: /usr/lib/python3.4/site-packages
Requires: pytz
Required-by: django-redis
```

从其中的：

`/usr/lib/python3.4/site-packages`

可以得知：

* 当前Python是：`/usr/lib/python3.4`
* 对应`site-packages`的位置是：`/usr/lib/python3.4/site-packages`
