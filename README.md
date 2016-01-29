Select language
---------------

  * [English](README/en-ww.md)
  * [中文（简体）](README/zh-cn.md)
  * [中文（繁体）](README/zh-tw.md)


Description
-----------

Hosts an extension system files, it is mainly to speed up the domain name resolution, but also can shield the site, etc..

![](README/img/logo.gif) will continue to update the latest and available hosts files. Includeing Google, Gmail, Android, Android Developers, Google Scholar, Google Developers, Google Play, Youtube, Facebook, Twitter, Amazon, Yahoo, Wikipedia, Github, Archive, Battle.NET, Box.com, BundleStars, DeviantART, DuckDuckGo, HumbleBundle, imgur, Indiegala, inoreader, Instagram, Ixquick, Logmein, MEGA, OneDrive, osu, RockStar, SoundCloud, Speedtest, Startpage, Steam, WordPress, XDA, Appannie, Travis CI fastly CDN and so on hosts.

**Note:**

Google, Gmail, Twitter, Facebook, etc are using HTTPS. Generally these sites are SSL encryption, eg:https://twitter.com/.

If you do not like to use [https://www.google.com.hk](https://www.google.com.hk/), you can use [https://www.google.com/ncr](https://www.google.com/ncr).

Possible areas of network (railcom, China unicom), This `hosts` file will be unable to use.

Due to DNS pollution is too serious, YouTube can only open the web page, the video can not play. If you want to watch YouTube video, you can use [YouTube Video Converter - Convert to MP3, MP4, AVI, MKV](http://www.onlinevideoconverter.com/video-converter) to download.


**Important things are to be repeated for 3 times:**

![](README/img/logo.gif) provided by the hosts is limited to study and research use, please do not used for any commercial purposes.

![](README/img/logo.gif) provided by the hosts is limited to study and research use, please do not used for any commercial purposes.

![](README/img/logo.gif) provided by the hosts is limited to study and research use, please do not used for any commercial purposes.



**※** ![](README/img/logo.gif) guarantee that in the hosts file does not add screen advertising items, don't hijack any web site, is not to install the back door.


Working Principles
------------------

Browser to access web site, first by the DNS server to access the website domain name resolution as a unique IP address, after the browser to this site to locate and access the data.

Operating system, regulations on DNS request before, first check whether his Hosts file with the domain name and IP mapping relationship. If it has direct access to the IP address specified by the network location, if not, then put forward to known the DNS server domain name resolution requests. That is to say, the Hosts IP parsing priority is higher than the DNS.

The applicable system
---------------------

  * Unix
  * Linux
  * Android
  * Mac
  * Windows

Update Address
--------------

  * [liuker0x007/hosts: Liuker Teamwill continue to update the latest and available hosts files...](https://github.com/liuker0x007/hosts)
  
How to modify the Hosts file
----------------------------

### Linux or Unix
If the system is Linux or Unix, have two ways.

**1.Use terminal:**  

Use wget or curl，eg:   
Open Terminal(Hot key: "Ctrl + Alt + T"), input `bash -c 'wget https://github.com/liuker0x007/hosts/blob/master/hosts -qO /tmp/hosts && sudo mv /tmp/hosts /etc/hosts'`.

**2.Not use terminal:**

Open the `/etc/hosts` folder，use downloaded `hosts` file to paste or override `hosts` file. Then, open Terminal that input `sudo systemctl restart NetworkManager` to entry into force.

**Note: If the system is Non-systemd Release, yon should input `sudo rcnscd restart`. If you are not sure, please try both again.**

### Android
If the system is Android, use RootExplore to open the `/system/etc/hosts` folder, use downloaded `hosts` file to paste or override `hosts` file. Then, the way is `开启飞行模式` -> `关闭飞行模式` to entry into force.

### Mac
If the system is Mac OS, open Finder. Then, press hot key is "Shift+Command+G" to find files, and input is `/etc/hosts`, use downloaded `hosts` file to paste or override `hosts` file. Finally, open Terminal that input `sudo killall -HUP mDNSResponder` to entry into force.

### Windows
If the system is Windwos, open the `C:\Windows\System32\drivers\etc` folder, use downloaded `hosts` file to paste or override `hosts` file. Finally, the way is ```开始 -> 运行 -> 输入cmd -> 在CMD窗口输入ipconfig /flushdns``` to entry into force.


**Note: If the `hosts` file have any content, you must add the content to at the end of this file。**

Update time
-----------

Updated almost every weekend.

Contact me
----------

  * E-mail：lzq@liuker.xyz
  * QQ：2523417411
