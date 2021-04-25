# pip show

可以用

```bash
pip show
```

去查看已安装的库/包的详细信息。

语法：

```bash
pip show xxx
```

## `pip show`举例

### Django

```bash
[root@xx-general-01 xxx]# pip3 show Django
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

### supervisor

```bash
[root@xx-general-01 robotDemo]# pip show supervisor
Name: supervisor
Version: 3.3.4
Summary: A system for controlling process state under UNIX
Home-page: http://supervisord.org/
Author: Chris McDonough
Author-email: chrism@plope.com
License: BSD-derived (http://www.repoze.org/LICENSE.txt)
Location: /usr/lib/python2.7/site-packages
Requires: meld3
Required-by: 
```

### kafka

```bash
# pip3 show kafka
Name: kafka
Version: 1.3.5
Summary: Pure Python client for Apache Kafka
Home-page: https://github.com/dpkp/kafka-python
Author: Dana Powers
Author-email: dana.powers@gmail.com
License: Apache License 2.0
Location: /usr/local/lib/python3.6/site-packages
Requires: 
Required-by:
```

### flask

```bash
(xxx) ➜  xxx pip show flask
Metadata-Version: 2.0
Name: Flask
Version: 0.11.1
Summary: A microframework based on Werkzeug, Jinja2 and good intentions
Home-page: http://github.com/pallets/flask/
Author: Armin Ronacher
Author-email: armin.ronacher@active-4.com
Installer: pip
License: BSD
Location: /root/Envs/xxx/lib/python2.7/site-packages
Requires: itsdangerous, Jinja2, Werkzeug, click
Classifiers:
  Development Status :: 4 – Beta
  Environment :: Web Environment
  Intended Audience :: Developers
  License :: OSI Approved :: BSD License
  Operating System :: OS Independent
  Programming Language :: Python
  Programming Language :: Python :: 2
  Programming Language :: Python :: 2.6
  Programming Language :: Python :: 2.7
  Programming Language :: Python :: 3
  Programming Language :: Python :: 3.3
  Programming Language :: Python :: 3.4
  Programming Language :: Python :: 3.5
  Topic :: Internet :: WWW/HTTP :: Dynamic Content
  Topic :: Software Development :: Libraries :: Python Modules
Entry-points:
  [console_scripts]
  flask=flask.cli:main
```
