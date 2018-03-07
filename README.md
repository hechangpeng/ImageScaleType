---
title: ImageView的ScaleType属性总结
date: 2017-10-27 10:29:53
tags:
categories: Android
---
<img src="http://owiq5fnuk.bkt.clouddn.com/2.jpg"/>
scaleType是个很有意思的属性，也是在图片显示处理场景中经常使用到的一个属性。因此有必要补充这个属性的知识。
android:scaleType="center"
原图居中显示在ImageView，小了不变，大了则裁剪。
<!-- more -->

android:scaleType="centerCrop"
原图居中显示在ImageView，小了则拉伸，大了则裁剪。

android:scaleType="centerInside"
原图居中显示在ImageView，小了不变，大了则按比例缩小。

android:scaleType="matrix"
从ImageView的左上角开始绘制，原图大了则裁剪。

android:scaleType="fitCenter"
原图居中显示在ImageView，小了则放缩，大了也放缩，注意：此处仅是放缩原图高度，宽度是不变的。

android:scaleType="fitEnd"
原图显示在ImageView的右内侧，小了则放缩，大了也放缩，注意：此处仅是放缩原图高度，宽度不变。

android:scaleType="fitStart"
原图显示在ImageView的左内侧，小了则放缩，大了也放缩，注意：此处仅是放缩原图高度，宽度不变。

android:scaleType="fitXY"
原图填充ImageView，不按比例放缩，直到填满为止。
