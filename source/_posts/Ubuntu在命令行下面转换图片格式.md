---
title: Ubuntu在命令行下面转换图片格式
date: 2017-03-23 19:04:39
tags: 菜鸟修炼
---

## Ubuntu在命令行下面转换图片格式 。 
- 尽管你可以使用GIMP来进行图纸格式的转换，但是操作还是有的麻烦。一个比较容易的方法是使用Imagemagick软件。安装完成以后，就可以使用convert命令。convert命令非常简单，譬如：
convert filename.jpg filename.bmp
　　
- 如果你使用JPEG等大小和图片质量有关的图形格式化，可以使用-quality参数。参数的数值在0至100之间，数值越大文件越大，通常情况下，60-80就可以了，譬如：
convert -quality 80 filename.bmp filename.jpg
