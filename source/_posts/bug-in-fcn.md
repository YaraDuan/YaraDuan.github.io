---
title: FCN for semantic-image-segmentation task中踩的坑
date: 2017-05-31 13:12:43
tags: 图象分割
categories: caffe
thumbnail: ./2017/05/31/bug-in-fcn/banner.jpg
---

最近在用FCN做一些分割任务，在跑已有demo的过程中就出现了很多坑了，虽然初识FCN，但还是要勇敢将坑踩下去。希望这篇blog更完的时候，我能有更大的进步~~~

#### **训练过程中出现shape不匹配**

开始使用voc-fcn-alexnet进行训练，训练过程中报错

```$xslt
F0531 21:29:22.348371  6780 net.cpp:765] Cannot copy param 0 weights from layer ‘fc6’; shape mismatch.  Source param shape is 4096 256 6 6 (37748736); target param shape is 4096 512 7 7 (102760448). To learn this layer’s parameters from scratch rather than copying from a saved net, rename the layer.
```

是因为pre-trained的参数数量和训练的alexnet-FCN参数数量不匹配，应用surgery.transplant函数把两个网格的参数统一起来。

