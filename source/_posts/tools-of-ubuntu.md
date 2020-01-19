---
title: ubuntu实用小工具
date: 2020-01-19 18:41:09
tags:
categories: tools
thumbnail: ./2020/01/19/tools-of-ubuntu/banner.svg
---

有一丢丢空余时间，又来搬运我印象笔记的内容到博客啦～

### 1、搜狗拼音

网上很多教程，很容易安装～

### 2、wps 

wps for linux下载地址： https://www.wps.cn/product/wpslinux/#

### 3、ubuntu主题美化

ref: https://www.jianshu.com/p/4a1c024d37bc

安装unity tweak tool图形化管理工具:
```$xslt
sudo apt-get install unity-tweak-tool
```

下载Flatabulous主题
```$xslt
sudo add-apt-repository ppa:noobslab/themes
sudo apt-get update
sudo apt-get install flatabulous-theme

```

下载配套图标
```$xslt
sudo add-apt-repository ppa:noobslab/icons
sudo apt-get update
sudo apt-get install ultra-flat-icons
```

打开unity tweak tool工具，修改主题为flatabulous，修改图标为ultra-flat

效果如下：
{% asset_img 1.png %}

### 4、迅雷

ref:  https://www.jianshu.com/p/6823685c739b?utm_source=oschina-app
     https://github.com/Xinkai/XwareDesktop/wiki/Ubuntu%E4%B8%8A%E7%BC%96%E8%AF%91%E5%AE%89%E8%A3%85%E8%AF%B4%E6%98%8E
     
### 5、便笺小工具

```$xslt
sudo add-apt-repository ppa:umang/indicator-stickynotes
sudo apt-get update
sudo apt-get install indicator-stickynotes
```

### 6、微信

```$xslt
ref: https://www.jianshu.com/p/f7ac9970b24f
sudo apt install snapd snapd-xdg-open
sudo snap install electronic-wechat
```

### 7、pdf阅读器

```$xslt
sudo apt-get install okular
```

搭配stardict读论文时可划词翻译

### 8、英汉词典

取词翻译很好用

```$xslt
sudo apt-get install stardict
```

download.huzheng.org/zh_CN/  下载词典并解压缩
将解压过的文件复制至 ～/.stardict/dic 文件夹下

### 9、meld

文件差异对比软件
```$xslt
sudo apt-get install meld
```
