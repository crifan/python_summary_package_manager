# pip list

可以用

```bash
pip list
```

来查看当前（Python）环境中的已安装的Python库（及其版本信息）

## `pip list`举例

```bash
 ⚙ limao@xxx  ~  pip list
Package           Version    Location
----------------- ---------- ---------------------------------------------------------
adbutils          0.7.1
apkutils2         1.0.0
asn1crypto        1.3.0
attrdict          2.0.1
attrs             19.3.0
Automat           20.2.0
autopep8          1.4.4
beautifulsoup4    4.8.2
blinker           1.4
Brotli            1.0.7
bs4               0.0.1
cached-property   1.5.1
certifi           2019.11.28
cffi              1.14.0
chardet           3.0.4
cigam             0.0.3
Click             7.0
constantly        15.1.0
cryptography      2.4.2
cssselect         1.1.0
decorator         4.4.1
defusedxml        0.6.0
Deprecated        1.2.7
deprecation       2.0.7
facebook-wda      1.3.4
Flask             1.1.1
Flask-Login       0.5.0
future            0.18.2
greenlet          1.0.0
h11               0.9.0
h2                3.1.1
hpack             3.0.0
humanize          0.5.1
hyperframe        5.2.0
hyperlink         19.0.0
idna              2.8
incremental       17.5.0
itemadapter       0.1.0
itsdangerous      1.1.0
Jinja2            2.11.1
json5             0.9.5
kaitaistruct      0.8
ldap3             2.6.1
logzero           1.5.0
lxml              4.5.0
MarkupSafe        1.1.1
mitmproxy         5.0.1
numpy             1.18.1
packaging         20.1
pandas            0.24.2
parsel            1.6.0
passlib           1.7.2
PGet              0.5.0
Pillow            7.0.0
pip               21.0.1
pipenv            2018.11.26
playwright        1.10.0
progress          1.5
Protego           0.1.16
protobuf          3.10.0
publicsuffix2     2.20191221
py                1.8.1
pyasn1            0.4.8
pyasn1-modules    0.2.8
pycodestyle       2.5.0
pycparser         2.19
pycurl            7.43.0.5
PyDispatcher      2.0.5
pyee              8.1.0
pyelftools        0.26
PyHamcrest        2.0.2
pyOpenSSL         19.0.0
pyparsing         2.4.6
pyperclip         1.7.0
pyquery           1.4.1
pyspider          0.3.10
python-dateutil   2.8.1
pytz              2019.3
PyYAML            5.3
queuelib          1.5.0
requests          2.22.0
retry             0.9.2
ruamel.yaml       0.16.7
Scrapy            2.2.1
service-identity  18.1.0
setuptools        41.2.0
six               1.14.0
sortedcontainers  2.1.0
soupsieve         1.9.5
spark-parser      1.8.9
tblib             1.7.0
tornado           4.5.3
tushare           1.2.48
Twisted           20.3.0
typing-extensions 3.7.4.3
u-msgpack-python  2.6.0
uiautomator2      2.5.3
uncompyle6        3.6.2      /Users/limao/dev/tools/python_decompile/python-uncompyle6
urllib3           1.25.8
urwid             2.0.1
virtualenv        16.7.9
virtualenv-clone  0.5.3
w3lib             1.22.0
weditor           0.4.2
Werkzeug          1.0.0
wheel             0.35.1
whichcraft        0.6.1
wrapt             1.11.2
WsgiDAV           3.0.3
wsproto           0.14.1
xdis              4.2.2
xmltodict         0.12.0
zope.interface    5.1.0
zstandard         0.12.0
```


另外一个`pipenv`的虚拟环境中的例子：

```bash
➜  tensorflow pip list --format=columns
Package                       Version
----------------------------- ---------
asn1crypto                    0.24.0
astroid                       1.5.3
attrs                         17.3.0
Automat                       0.6.0
backports.functools-lru-cache 1.4
browsermob-proxy              0.8.0
certifi                       2017.11.5
cffi                          1.11.2
chardet                       3.0.4
configparser                  3.5.0
constantly                    15.1.0
cryptography                  2.1.4
cssselect                     1.0.1
enum34                        1.1.6
hyperlink                     17.3.1
idna                          2.6
incremental                   17.5.0
ipaddress                     1.0.19
isort                         4.2.15
lazy-object-proxy             1.3.1
lxml                          4.1.1
mccabe                        0.6.1
parsel                        1.2.0
pip                           9.0.1
pyasn1                        0.4.2
pyasn1-modules                0.2.1
pycparser                     2.18
PyDispatcher                  2.0.5
pylint                        1.7.2
pyOpenSSL                     17.5.0
queuelib                      1.4.2
requests                      2.18.4
Scrapy                        1.4.0
selenium                      3.7.0
service-identity              17.0.0
setuptools                    38.4.0
singledispatch                3.4.0.3
six                           1.10.0
speedtest-cli                 1.0.7
Twisted                       17.9.0
urllib3                       1.22
virtualenv                    15.1.0
w3lib                         1.18.0
wheel                         0.30.0
wrapt                         1.10.11
zope.interface                4.4.3
```
