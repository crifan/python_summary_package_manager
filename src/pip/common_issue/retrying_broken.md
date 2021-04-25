# Retrying after connection broken by NewConnectionError

**现象**：

```bash
pip install boto3
```

报错：

```bash
(RunningFast) ➜  stable pip install boto3
Collecting boto3
  Retrying (Retry(total=4, connect=None, read=None, redirect=None)) after connection broken by ‘NewConnectionError(‘<pip._vendor.requests.packages.urllib3.connection.VerifiedHTTPSConnection object at 0x7f30c47e8710>: Failed to establish a new connection: [Errno -2] Name or service not known’,)’: /simple/boto3/
...
  Retrying (Retry(total=0, connect=None, read=None, redirect=None)) after connection broken by ‘NewConnectionError(‘<pip._vendor.requests.packages.urllib3.connection.VerifiedHTTPSConnection object at 0x7f30c306b5d0>: Failed to establish a new connection: [Errno -2] Name or service not known’,)’: /simple/boto3/
  Could not find a version that satisfies the requirement boto3 (from versions: )
No matching distribution found for boto3

Failed to establish a new connection Errno -2  Name or service not known

Retrying (Retry(total=4, connect=None, read=None, redirect=None)) after connection broken by ‘NewConnectionError(‘<pip._vendor.requests.packages.urllib3.connection.VerifiedHTTPSConnection object at 0x7f30c47e8710>: Failed to establish a new connection: [Errno -2] Name or service not known’,)’: /simple/boto3/
```

**原因**：当时网络不稳定，连不上pip的源，导致报网络相关的错误

**解决办法**：

* 换个时间（网络就正常了）
  * 此处当时就是这么做的：换了个时间，第二天早上，网络正常了，再去`pip install boto3`，就可以了
* 给pip加上代理
  * 确保可以正常访问pip的源
    * 如何操作，详见前面章节：[给pip加代理](../../pip/commands/pip_install/download_speedup/add_proxy.html)
