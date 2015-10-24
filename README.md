说明
----

hosts文件是一个没有扩展名的系统文件，它的主要作用是能加快域名解析，还可以屏蔽网站等。 

持续更新Google、Gmail、谷歌学术、Google Play、Facebook、Twitter、Youtube、Android、亚马逊、雅虎、维基百科、Mozilla、Github、、Archive、Battle.NET、Box.com、BundleStars、DeviantART、DuckDuckGo、HumbleBundle、imgur、Indiegala、inoreader、Instagram、Ixquick、Logmein、MEGA、OneDrive、osu、RockStar、SoundCloud、Speedtest、Startpage、Steam、WordPress、XDA、Appannie、Travis CI fastly CDN、Google Services、Google apis、Google Drive、Googl eusercontent、Gstatic、Google other等hosts。

工作原理
--------

浏览器访问网站，要首先通过DNS服务器把要访问的网站域名解析成一个唯一的IP地址，之后，浏览器才能对此网站进行定位并且访问其数据。

操作系统规定，在进行DNS请求以前，先检查系自己的Hosts文件中是否有这个域名和IP的映射关系。如果有，则直接访问这个IP地址指定的网络位置，如果没有，再向已知的DNS服务器提出域名解析请求。也就是说Hosts的IP解析优先级比DNS要高。

适用系统
--------
  
  * Unix
  * Linux
  * Android
  * Mac
  * Windows

更新地址
--------

提供了下面两个更新地址：

  * [hosts_免费高速下载|百度云 网盘-分享无限制](http://pan.baidu.com/s/1kTlKev9)
  * [liuker0x007/hosts - Github](https://github.com/liuker0x007/hosts)
  
使用方法
--------

### Unix
如果是Unix系统，打开`/etc/hosts`目录，把下载好的`hosts`文件粘帖和覆盖该目录的`hosts`文件。

### Linux
如果是Linux系统，打开`/etc/hosts` 目录，把下载好的`hosts`文件粘帖和覆盖该目录的`hosts`文件。

### Android
如果是Android系统，用 RE管理器 （前提需要手机已Root）打开`/system/etc/hosts`目录，把下载好的`hosts`文件粘帖和覆盖该目录的`hosts`文件。

### Mac
如果是Mac系统，打开你的文件管理器（也就是Finder），然后，请按快捷键组合“Shift+Command+G”三个组合按键查找文件，并输入Hosts文件的所在路径：`/etc/hosts`，把下载好的`hosts`文件粘帖和覆盖该目录的`hosts`文件。

### Windows
如果是Windows系统，打开`C:\WINDOWS\system32\drivers\etc`目录，把下载好的`hosts`文件粘帖和覆盖该目录的`hosts`文件。

注：如果`hosts`文件中有内容，请把它追加到`hosts`文件末尾。

更新时间
--------

基本上每周都会更新一次。
