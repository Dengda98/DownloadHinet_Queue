基于[HinetPy](https://github.com/seisman/HinetPy)的***多账户队列式并行下载*** [NIED Hi-net](https://www.hinet.bosai.go.jp/) 地震数据脚本。  

    实际手动下载会发现，在你本地网速正常的情况下，当你在Hinet官网发出下载请求后，大部分事件是在等待Hinet服务器整理数据，然后才能下载。

    该脚本通过使用多账号，将下载任务以队列的形式进行多进程并行下载，提高下载效率。

+ 安装依赖  
要求安装[HinetPy](https://github.com/seisman/HinetPy)程序包和Hinet官网提供的[win32tools](https://hinetwww11.bosai.go.jp/auth/manual/?LANG=en)工具包

+ 参数设置  
在脚本中提前设置好相关参数，包括多个磁盘的下载路径，多个账户密码，事件目录等。