语言选择
--------

  * [English](README/en-ww.md)
  * [中文（简体）](README/zh-cn.md)


说明
----

想上Google者，请上[https://liuker.xyz](https://liuker.xyz) , 无需修改hosts文件！

适用系统
--------

  * Unix
  * Linux
  * Android
  * Mac
  * Windows

更新地址
--------

  * [liuker0x007/hosts: Liuker Teamwill continue to update the latest and available hosts files...](https://github.com/liuker0x007/hosts)
  
如何修改Hosts
-------------

### Linux & Unix
如果是Linux或者Unix系统，有两种方法。

**1、终端：**  

使用wget或curl，以wget为例：  
开启终端（快捷键为“Ctrl + Alt + T”）输入`bash -c 'wget https://raw.githubusercontent.com/liuker0x007/hosts/master/hosts -qO /tmp/hosts && sudo mv /tmp/hosts /etc/hosts'`。

**2、非终端：**

打开`/etc/hosts`目录，用下载好的`hosts`文件粘帖和覆盖该目录的`hosts`文件。最后在终端输入`sudo systemctl restart NetworkManager`。

**注意 : 非systemd发行版，终端输入`sudo rcnscd restart`，如果不清楚请两个都试一次。**

### Android
如果是Android系统，用RE管理器（前提需要手机已Root）打开`/system/etc/hosts`目录，用下载好的`hosts`文件粘帖和覆盖该目录的`hosts`文件。然后通过`开启飞行模式` -> `关闭飞行模式`的方式使其生效。

### Mac
如果是Mac系统，打开你的文件管理器（也就是Finder），然后，请按快捷键组合“Shift+Command+G”三个组合按键查找文件，并输入Hosts文件的所在路径：`/etc/hosts`，用下载好的`hosts`文件粘帖和覆盖该目录的`hosts`文件。然后终端输入`sudo killall -HUP mDNSResponder`使其生效。

### Windows
如果是Windows系统，用文本编辑器(如Notepad++|记事本)打开`C:\Windows\System32\drivers\etc`中的`hosts`文件，用下载好的`hosts`文件全部内容复制到`C:\WINDOWS\system32\drivers\etc`目录中的`hosts`文件中。或者用下载好的`hosts`文件粘帖和覆盖`C:\WINDOWS\system32\drivers\etc`目录中的`hosts`文件中。保存后通过```开始 -> 运行 -> 输入cmd -> 在CMD窗口输入ipconfig /flushdns```使其生效。

注意：如果遇到无法保存，请右键hosts -> 属性 -> 安全，然后选择你登陆的用户名，最后点击编辑，勾选"写入"即可。

**注意：如果`hosts`文件中已经有内容，那么请把已有的内容追加到`hosts`文件末尾。**

更新时间
--------

基本上每周周末都会更新一次。

联系方式
--------

  * E-mail: [lt@liuker.xyz](mailto:lt@liuker.xyz)
  * QQ: [2523417411](http://wpa.qq.com/msgrd?v=3&uin=2523417411&site=qq&menu=yes)
