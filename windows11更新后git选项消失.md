## windows11更新后右键的git选项消失

在windows内搜索注册表，打开，找到/HKEY_CLASSES_ROOT/Directory/Background/shell

新建Key，名字为open in git，将默认修改为Git Bash Here

新建String Value，名字为Icon，值为D:\Git\git-bash.exe，**是你的git.exe的路径**

在此Key内新建Key，名字为command，默认值为D:\Git\git-bash.exe，也是**你的git.exe的路径**

![gitzcb1](img/gitzcb1.png)

![gitzcb2](img/gitzcb2.png)
