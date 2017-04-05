---
title: 解决在ubuntu中打开WPS时出现的系统缺失字体问题
date: 2017-03-24 22:16:15
tags: 菜鸟修炼
---
解决打开WPS时出现的系统缺失字体问题：
下载
https://pan.baidu.com/s/1eS6xIzo
wps_symbol_fonts.zip
 
将wps_symbol_fonts.zip解压

cd wps_symbol_fontsls
 将目录中所有文件复制到/usr/share/fonts下：
sudo cp mtextra.ttf  symbol.ttf  WEBDINGS.TTF  wingding.ttf  WINGDNG2.ttf  WINGDNG3.ttf  /usr/share/fonts

重新打开WPS，问题解决。
另外，安装完WPS后就没有必要保留libreOffice
卸载libreOffice：
sudo apt-get remove libreoffice-common
顺便把Amazon链接删除了吧：
- sudo apt-get remove unity-webapps-common
- sudo apt autoremove
