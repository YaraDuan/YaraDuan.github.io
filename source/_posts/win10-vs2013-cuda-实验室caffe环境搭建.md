---
title: win10+vs2013+cuda 实验室caffe环境搭建
date: 2017-04-09 14:24:36
tags: 给脑子不好的我留的特别关怀
categories: caffe
thumbnail: ./2017/04/09/win10-vs2013-cuda-实验室caffe环境搭建/banner.jpeg
---
不得已，又重新复习了下怎么搭建实验室的caffe环境，脑子不好使，还是要把句句话记下来啊喂~ 

#### **安装matlab**

先要安装vs2013，有需要的也可以顺带把matlab安上，按完matlab要记得配环境啊~
Path中添加：

```
D:\Program Files\MATLAB\R2016b\runtime\win64
D:\Program Files\MATLAB\R2016b\bin
D:\Program Files\MATLAB\R2016b\polyspace\bin
```


#### **下载cuda并安装**

在安装cuda之前先要安装驱动，这里是英伟达960~

下载地址: http://www.nvidia.cn/Download/index.aspx?lang=cn

接下来就是安装cuda以及配置cuda环境，话不多说，参考这篇博客就好啦: http://blog.csdn.net/u011821462/article/details/50145221

这篇文章写得十分详细，按照这个步骤来应该没什么问题哒~

在安装cuda的时候，可能会遇到安装失败的问题，说你一堆东西没安装，其实安装驱动的时候已经安装过了，这里为什么这样提示我也不知道~ 安装时选择自定义安装，然后只勾选CUDA选项进行安装就好了，实际上也只需要CUDA~


#### **安装miniconda2**

下载地址： https://conda.io/miniconda.html

安装后，配环境~ 在Path中添加：

```
C:\ProgramData\miniconda2
C:\ProgramData\miniconda2\Scripts
C:\ProgramData\miniconda2\Library\bin
```


#### **跑跑项目试试**

打开/caffe-windows/windows下的caffe.sln

在跑项目前，更改/caffe-windows/windows下的CommonSettings文件中的相关配置，如CUDA的版本号，cudann的路径，miniconda的路径，matlab路径等

跑跑项目没什么问题，就继续往下走~

打开vs，安装Python Tools for Visual Studio

打开项目test，根据项目中引用的包，安装依赖包

记得把caffe包放在项目目录下~ 或是设置路径

安装到graphviz时，记得配环境~ Path添加：

```
C:\ProgramData\Miniconda2\Library\bin\graphviz
```

所有包安好后，跑一下，没问题就大功告成啦~






