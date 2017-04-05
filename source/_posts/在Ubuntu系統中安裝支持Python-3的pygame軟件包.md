---
title: 在Ubuntu系統中安裝支持Python 3的pygame軟件包
date: 2017-03-23 22:29:36
tags: 菜鸟修炼
---

打開終端機（Terminal，也稱為終端）
依次執行下列六條命令：
- sudo apt-get install mercurial
- hg clone https://bitbucket.org/pygame/pygame
- cd pygame
- sudo apt-get install python3-dev python3-numpy libsdl-dev libsdl-image1.2-dev \
libsdl-mixer1.2-dev libsdl-ttf2.0-dev libsmpeg-dev libportmidi-dev \
libavformat-dev libswscale-dev libjpeg-dev libfreetype6-dev
- python3 setup.py build
- sudo python3 setup.py install
執行第二条命令之前，如果當前目錄下已經有了名叫pygame的子目錄，那麼就請先把該子目錄中的內容備份好，然後刪除這個pygame子目錄，刪除完之後，執行該命令。
第二條命令如果在執行的時候卡住，那就請按Ctrl+C鍵中止它，然後重新執行該命令。
參考資料：
http://askubuntu.com/questions/401342/how-to-download-pygame-in-python3-3

