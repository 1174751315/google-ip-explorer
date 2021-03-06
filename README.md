google-ip-explorer
==================

由于最近GFW姨妈来得比较频繁, 所以写了个小工具. 这工具能够找出可用的Google IP地址.

## 教程

[Google IP Explorer](https://github.com/PeerXu/google-ip-explorer)是一个查找Google IP列表的工具. 可以单独使用, 也可以配合Goagent使用.

如果已经安装了gevent库, 那么可以大大地增加查找速度.

    $ git clone https://github.com/PeerXu/google-ip-explorer.git
    $ cd google-ip-explorer
    $ python google.py input.txt

Google IP列表就在output.txt文件中.

如果你需要直接使用, 那么就挑一个IP直接在浏览器里面就能使用了.

如果你需要和Goagent配合使用的话, 那么就将```proxy.ini``` 下的```[iplist]``` 下的```google_cn``` 和 ```google_hk``` 替换为output.txt的内容就可以了~

##另外一个查找可用的Google IP的方法
1. 打开[ZoomEye](http://www.zoomeye.org/)
2. 在搜索框里输入**gws**,点击搜索一下
3. 在返回的结果中选择一个ip，复制到浏览器的地址栏
4. enter，just enjoy it.

###或者跳过1-2步，直接点击以下链接:
[click here](http://www.zoomeye.org/search?q=gws)

然后再执行3-4步。

####ref： 
[what is ZoomEye?](http://www.zoomeye.org/about)


##编译成可以单独运行的.exe文件

使用PyInstaller将`google.py`打包成**win7 x86**环境下可以独立运行的exe文件。
只需直接下载`google`文件夹，然后在`google/dist/`路径下找到`google.exe`，双击运行。
运行结束后，`output.txt`中保存结果。

