語言選擇
--------

  * [English](en-ww.md)
  * [中文（简体）](zh-cn.md)
  * [中文（繁體）](zh-tw.md)


說明
----

hosts檔是一個沒有副檔名的系統檔，它的主要作用是能加快功能變數名稱解析，還可以遮罩網站等。 

![](img/logo.gif)將持續更新最新的且可用的hosts檔。其中包括Google, Gmail, Android, Android Developers, Google Scholar, Google Developers, Google Play, Youtube, Facebook, Twitter, Amazon, Yahoo, Wikipedia, Github, Archive, Battle.NET, Box.com, BundleStars, DeviantART, DuckDuckGo, HumbleBundle, imgur, Indiegala, inoreader, Instagram, Ixquick, Logmein, MEGA, OneDrive, osu, RockStar, SoundCloud, Speedtest, Startpage, Steam, WordPress, XDA, Appannie, Travis CI fastly CDN等hosts.

**注：**

Google、Gmail、維琪百科、Twitter、Facebook等都用https加密方式打開。一般這些網站都是SSL加密連結，如Twitter：https://twitter.com/。

如果不喜歡用穀歌香港，可以訪問[https://www.google.com/ncr](https://www.google.com/ncr)，No Country Redirect是禁止國別跳轉。

可能有的地區的網路（鐵通、聯通）hosts會出現無法正常使用！

由於DNS污染太嚴重，YouTube只能打開網頁，視頻無法播放！如果想觀看YouTube的視頻，可以通過[YouTube Video Converter - Convert to MP3, MP4, AVI, MKV](http://www.onlinevideoconverter.com/video-converter)網站下載視頻。


**重要的事情說三遍：**

![](img/logo.gif)團隊所提供的hosts僅限於學習和研究使用，請勿用於任何商業用途。

![](img/logo.gif)團隊所提供的hosts僅限於學習和研究使用，請勿用於任何商業用途。

![](img/logo.gif)團隊所提供的hosts僅限於學習和研究使用，請勿用於任何商業用途。


**※** ![](img/logo.gif)並且保證在hosts檔裡不會添加遮罩廣告條目，也不會劫持任何網站，更不會安裝後門。


工作原理
--------

流覽器訪問網站，要首先通過DNS伺服器把要訪問的網站功能變數名稱解析成一個唯一的IP位址，之後，流覽器才能對此網站進行定位並且訪問其資料。

作業系統規定，在進行DNS請求以前，先檢查系自己的Hosts檔中是否有這個功能變數名稱和IP的映射關係。如果有，則直接訪問這個IP位址指定的網路位置，如果沒有，再向已知的DNS伺服器提出功能變數名稱解析請求。也就是說Hosts的IP解析優先順序比DNS要高。

適用系統
--------

  * Unix
  * Linux
  * Android
  * Mac
  * Windows

更新位址
--------

  * * [liuker0x007/hosts: Liuker Teamwill continue to update the latest and available hosts files...](https://github.com/liuker0x007/hosts)
  
如何修改Hosts
--------

### Linux & Unix
如果是Linux或者Unix系統，有兩種方法。

**1、終端：**  

使用wget或curl，以wget為例：  
開啟終端（快速鍵為“Ctrl + Alt + T”）輸入`bash -c 'wget https://github.com/liuker0x007/hosts/blob/master/hosts -qO /tmp/hosts && sudo mv /tmp/hosts /etc/hosts'`。

**2、非終端：**

打開`/etc/hosts`目錄，用下載好的`hosts`檔粘帖和覆蓋該目錄的`hosts`檔。最後在終端輸入`sudo systemctl restart NetworkManager`。

**注意 : 非systemd發行版本，終端輸入`sudo rcnscd restart`，如果不清楚請兩個都試一次。**

### Android
如果是Android系統，用RE管理器（前提需要手機已Root）打開`/system/etc/hosts`目錄，用下載好的`hosts`檔粘帖和覆蓋該目錄的`hosts`檔。然後通過`開啟飛行模式` -> `關閉飛行模式`的方式使其生效。

### Mac
如果是Mac系統，打開你的檔案管理員（也就是Finder），然後，請按快速鍵組合“Shift+Command+G”三個組合按鍵查找檔，並輸入Hosts檔的所在路徑：`/etc/hosts`，用下載好的`hosts`檔粘帖和覆蓋該目錄的`hosts`檔。然後終端輸入`sudo killall -HUP mDNSResponder`使其生效。

### Windows
如果是Windows系統，用文字編輯器(如Notepad++|記事本)打開`C:\Windows\System32\drivers\etc`中的`hosts`檔，用下載好的`hosts`檔全部內容複製到`C:\WINDOWS\system32\drivers\etc`目錄中的`hosts`檔中。或者用下載好的`hosts`檔粘帖和覆蓋`C:\WINDOWS\system32\drivers\etc`目錄中的`hosts`檔中。保存後通過```開始 -> 運行 -> 輸入cmd -> 在CMD視窗輸入ipconfig /flushdns```使其生效。

注意：如果遇到無法保存，請右鍵hosts -> 屬性 -> 安全，然後選擇你登陸的用戶名，最後點擊編輯，勾選"寫入"即可。

**注意：如果`hosts`檔中已經有內容，那麼請把已有的內容追加到`hosts`檔末尾。**

更新時間
--------

基本上每週週末都會更新一次。

聯繫方式
--------

  * E-mail：lzq@liuker.xyz
  * QQ：[2523417411](http://wpa.qq.com/msgrd?v=3&uin=2523417411&site=qq&menu=yes)
