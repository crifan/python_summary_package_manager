# 给pip加代理

此处也可以通过给pip加代理的方式实现加速pip下载。

实现方式：用`pip`安装时，加上代理：

```bash
pip --proxy http://127.0.0.1:1087 install pandas
```

其中：

* 代理地址：`127.0.0.1:1087`
  * 对应着此处本地的`ss`的`http代理`：
    * ![local_ss_http_proxy](../../../../assets/img/local_ss_http_proxy.png)
