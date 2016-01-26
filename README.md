说明
----

hosts文件是一个没有扩展名的系统文件，它的主要作用是能加快域名解析，还可以屏蔽网站等。 

![](img/]LT[.gif)团队将持续更新Google、Gmail、谷歌学术、Google Play、Facebook、Twitter、Youtube、Android、亚马逊、雅虎、维基百科、Mozilla、Github、、Archive、Battle.NET、Box.com、BundleStars、DeviantART、DuckDuckGo、HumbleBundle、imgur、Indiegala、inoreader、Instagram、Ixquick、Logmein、MEGA、OneDrive、osu、RockStar、SoundCloud、Speedtest、Startpage、Steam、WordPress、XDA、Appannie、Travis CI fastly CDN等hosts。

**注：**

Google、Gmail、维基百科、Twitter、Facebook等都用https加密方式打开。（一般这些网站都是SSL加密链接，如Twitter：https://twitter.com/）

如果不喜欢用谷歌香港，可以以[https://www.google.com/ncr](https://www.google.com/ncr)方式访问，（No Country Redirect）禁止国别跳转。

可能有的地区的网络（铁通、联通）hosts会出现无法正常使用！

由于DNS污染太严重，YouTube只能打开网页，视频无法播放！如果想观看YouTube的视频，可以通过[YouTube Video Converter - Convert to MP3, MP4, AVI, MKV](http://www.onlinevideoconverter.com/video-converter)网站把视频下载下来，接着在本地观看。


**重要的事情说三遍：**

![](img/]LT[.gif)团队所提供的hosts仅限于学习和研究使用，请勿用于任何商业用途。

![](img/]LT[.gif)团队所提供的hosts仅限于学习和研究使用，请勿用于任何商业用途。

![](img/]LT[.gif)团队所提供的hosts仅限于学习和研究使用，请勿用于任何商业用途。

并且保证在hosts文件里不会添加屏蔽广告条目，也不会劫持任何网站，更不会安装后门。


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

  * [liuker0x007/hosts: Liuker Team团队将持续更新Goog... - GitHub](https://github.com/liuker0x007/hosts)
  
如何修改Hosts
--------

### Linux & Unix
**终端：**  

使用wget或curl，以wget为例：  
开启终端（快捷键为“Ctrl + Alt + T”）输入`bash -c 'wget https://github.com/liuker0x007/hosts/blob/master/hosts -qO /tmp/hosts && sudo mv /tmp/hosts /etc/hosts'`。

**非终端：**

打开`/etc/hosts`目录，把下载好的`hosts`文件粘帖和覆盖该目录的`hosts`文件。最后在终端输入`sudo systemctl restart NetworkManager`。

**注意 : 非systemd发行版，终端输入`sudo rcnscd restart`，如果不清楚请两个都试一次。**

### Android
如果是Android系统，用RE管理器（前提需要手机已Root）打开`/system/etc/hosts`目录，把下载好的`hosts`文件粘帖和覆盖该目录的`hosts`文件。然后通过`开启飞行模式` -> `关闭飞行模式`的方式使其生效。

### Mac
如果是Mac系统，打开你的文件管理器（也就是Finder），然后，请按快捷键组合“Shift+Command+G”三个组合按键查找文件，并输入Hosts文件的所在路径：`/etc/hosts`，把下载好的`hosts`文件粘帖和覆盖该目录的`hosts`文件。然后终端输入`sudo killall -HUP mDNSResponder`使其生效。

### Windows
用文本编辑器(如Notepad++|记事本)打开`C:\Windows\System32\drivers\etc`中的hosts文件，把下载好的`hosts`文件全部内容复制到`C:\WINDOWS\system32\drivers\etc`目录中的hosts文件中，保存后通过```开始 -> 运行 -> 输入cmd -> 在CMD窗口输入ipconfig /flushdns```使其生效。

注意：如果遇到无法保存，请右键hosts -> 属性 -> 安全，然后选择你登陆的用户名，最后点击编辑，勾选"写入"即可。

**注意：如果`hosts`文件中已经有内容，那么请把已有的内容追加到`hosts`文件末尾。**

更新时间
--------

基本上每周周末都会更新一次。

联系方式
--------

  * E-mail：lzq@liuker.xyz
  * QQ：[2523417411](http://wpa.qq.com/msgrd?v=3&uin=2523417411&site=qq&menu=yes)
