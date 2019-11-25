

#  pip install jupyter notebook 执行是遇到下面错误

ERROR: Command errored out with exit status 1: python setup.py egg_info Check the logs for full command output.
==
    numpy      1.17.4
    pip        19.3.1
    scipy      1.3.2
    setuptools 41.6.0

        
        python -m pip install --upgrade setuptools 
        python -m pip install --upgrade pip

        pip install --upgrade pip -vvv
        又安装 vc++14
# 卸载后C++ 2017 c++2014 通过builder 重新安装了C++组件 
# 都没有用.. :)
# 这个安装不了
        hon_dateutil-2.8.1-py2.py3-none-any.whl
        Collecting pywinpty>=0.5; os_name == "nt"
        Using cached https://files.pythonhosted.org/packages/21/ae/acbedcee475d049647e45ee949e23ca492764fcd8027a073fcf07646d47c/pywinpty-0.5.5.tar.gz

# 得知  pywinpty-0.5.5无法安装 
## 到[网站](https://www.lfd.uci.edu/~gohlke/pythonlibs/)上找wh1(关于py38的) 或者找关于这个的网站 :Unofficial Windows Binaries for Python Extension Packages 
        通过pip install XXXX.wh1 安装
        ex: pip install pywinpty-0.5.5-cp38-cp38-win_amd64.whl