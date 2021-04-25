# pip uninstall

* 卸载已安装的Python库
    ```bash
    pip uninstall xxx
    ```
* 有时候，pip会提示你，确认是否删除，需要输入`y`才能继续删除
  * 如果不希望被提示，直接删除，可以加上`y`
    ```bash
    pip uninstall -y xxx
    ```
* 想要卸载某个特定版本，可以指定版本号
    ```bash
    pip uninstall xxx==verion_number
    ```

## `pip uninstall`举例

* 卸载（已安装，但有问题的）pycurl
    ```bash
    pip uninstall pycurl
    ```
  * 不询问(是否删除)而直接删除
    ```bash
    pip uninstall -y pycurl
    ```
* 卸载uiautomator2
    ```bash
    pip uninstall uiautomator2
    ```
* 卸载facebook-wda
    ```bash
    pip uninstall facebook-wda
    ```
* 卸载`1.7.0rc1`版本的`tensorflow`
    ```bash
    pip uninstall tensorflow==1.7.0rc1
    ```
* 卸载pyinstaller
    ```bash
    pip uninstall pyinstaller
    ```
* 卸载pipenv
    ```bash
    pip3 uninstall pipenv
    ```
* 卸载pip自己
    ```bash
    python -m pip uninstall pip
    ```
* 卸载mime
    ```bash
    pip uninstall mime
    ```
* 卸载selenium
    ```bash
    pip uninstall selenium
    ```

### 给出部分库的详细卸载日志

* 卸载virtualenv
    ```bash
    pip uninstall virtualenv
    ```
    * 完整log举例
        ```bash
        ➜  virtualenv pip uninstall virtualenv
        Uninstalling virtualenv-15.1.0:
        /usr/local/bin/virtualenv
        /usr/local/lib/python2.7/site-packages/virtualenv-15.1.0.dist-info/DESCRIPTION.rst
        /usr/local/lib/python2.7/site-packages/virtualenv-15.1.0.dist-info/INSTALLER
        /usr/local/lib/python2.7/site-packages/virtualenv-15.1.0.dist-info/METADATA
        /usr/local/lib/python2.7/site-packages/virtualenv-15.1.0.dist-info/RECORD
        /usr/local/lib/python2.7/site-packages/virtualenv-15.1.0.dist-info/WHEEL
        /usr/local/lib/python2.7/site-packages/virtualenv-15.1.0.dist-info/entry_points.txt
        /usr/local/lib/python2.7/site-packages/virtualenv-15.1.0.dist-info/metadata.json
        /usr/local/lib/python2.7/site-packages/virtualenv-15.1.0.dist-info/top_level.txt
        /usr/local/lib/python2.7/site-packages/virtualenv.py
        /usr/local/lib/python2.7/site-packages/virtualenv.pyc
        /usr/local/lib/python2.7/site-packages/virtualenv_support/__init__.py
        /usr/local/lib/python2.7/site-packages/virtualenv_support/__init__.pyc
        /usr/local/lib/python2.7/site-packages/virtualenv_support/argparse-1.4.0-py2.py3-none-any.whl
        /usr/local/lib/python2.7/site-packages/virtualenv_support/pip-9.0.1-py2.py3-none-any.whl
        /usr/local/lib/python2.7/site-packages/virtualenv_support/setuptools-28.8.0-py2.py3-none-any.whl
        /usr/local/lib/python2.7/site-packages/virtualenv_support/wheel-0.29.0-py2.py3-none-any.whl
        Proceed (y/n)? y
        Successfully uninstalled virtualenv-15.1.0
        ```
        * 期间需要输入`y`才可继续卸载
          * 想要实现，不需要输入`y`就可以直接自动卸载，可以加上`-y`参数
            ```bash
            pip uninstall -y virtualenv
            ```
* 卸载supervisor
    ```bash
    pip2 uninstall supervisor
    ```
    * 详细日志
        ```bash
        [root@xxx-general-01 robotDemo]# pip2 uninstall supervisor
        Uninstalling supervisor-3.3.4:
        Would remove:
            /usr/bin/echo_supervisord_conf
            /usr/bin/pidproxy
            /usr/bin/supervisorctl
            /usr/bin/supervisord
            /usr/lib/python2.7/site-packages/supervisor-3.3.4-py2.7-nspkg.pth
            /usr/lib/python2.7/site-packages/supervisor-3.3.4-py2.7.egg-info
            /usr/lib/python2.7/site-packages/supervisor/childutils.py
            /usr/lib/python2.7/site-packages/supervisor/confecho.py
            /usr/lib/python2.7/site-packages/supervisor/datatypes.py
            /usr/lib/python2.7/site-packages/supervisor/dispatchers.py
            /usr/lib/python2.7/site-packages/supervisor/events.py
            /usr/lib/python2.7/site-packages/supervisor/http.py
            /usr/lib/python2.7/site-packages/supervisor/http_client.py
            /usr/lib/python2.7/site-packages/supervisor/loggers.py
            /usr/lib/python2.7/site-packages/supervisor/medusa/*
            /usr/lib/python2.7/site-packages/supervisor/options.py
            /usr/lib/python2.7/site-packages/supervisor/pidproxy.py
            /usr/lib/python2.7/site-packages/supervisor/poller.py
            /usr/lib/python2.7/site-packages/supervisor/process.py
            /usr/lib/python2.7/site-packages/supervisor/rpcinterface.py
            /usr/lib/python2.7/site-packages/supervisor/scripts/loop_eventgen.py
            /usr/lib/python2.7/site-packages/supervisor/scripts/loop_listener.py
            /usr/lib/python2.7/site-packages/supervisor/scripts/sample_commevent.py
            /usr/lib/python2.7/site-packages/supervisor/scripts/sample_eventlistener.py
            /usr/lib/python2.7/site-packages/supervisor/scripts/sample_exiting_eventlistener.py
            /usr/lib/python2.7/site-packages/supervisor/skel/sample.conf
            /usr/lib/python2.7/site-packages/supervisor/socket_manager.py
            /usr/lib/python2.7/site-packages/supervisor/states.py
            /usr/lib/python2.7/site-packages/supervisor/supervisorctl.py
            /usr/lib/python2.7/site-packages/supervisor/supervisord.py
            /usr/lib/python2.7/site-packages/supervisor/tests/*
            /usr/lib/python2.7/site-packages/supervisor/ui/images/button_refresh.gif
            /usr/lib/python2.7/site-packages/supervisor/ui/images/button_restart.gif
            /usr/lib/python2.7/site-packages/supervisor/ui/images/button_stop.gif
            /usr/lib/python2.7/site-packages/supervisor/ui/images/icon.png
            /usr/lib/python2.7/site-packages/supervisor/ui/images/rule.gif
            /usr/lib/python2.7/site-packages/supervisor/ui/images/state0.gif
            /usr/lib/python2.7/site-packages/supervisor/ui/images/state1.gif
            /usr/lib/python2.7/site-packages/supervisor/ui/images/state2.gif
            /usr/lib/python2.7/site-packages/supervisor/ui/images/state3.gif
            /usr/lib/python2.7/site-packages/supervisor/ui/images/supervisor.gif
            /usr/lib/python2.7/site-packages/supervisor/ui/status.html
            /usr/lib/python2.7/site-packages/supervisor/ui/stylesheets/supervisor.css
            /usr/lib/python2.7/site-packages/supervisor/ui/tail.html
            /usr/lib/python2.7/site-packages/supervisor/version.txt
            /usr/lib/python2.7/site-packages/supervisor/web.py
            /usr/lib/python2.7/site-packages/supervisor/xmlrpc.py
        Proceed (y/n)? y
        Successfully uninstalled supervisor-3.3.4
        ```

