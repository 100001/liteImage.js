liteImage.js
============
###说明
-----
* 该组件基于 jQuery or Zepto 实现。

* 图片压缩完后，其压缩结果的size不一定会比原图小（主要是图片本身size比较小（几十K or 几K）的时候），这个时候返回结果存的是原始图片文件，类型为File，如果是压缩后的图片是Blob类型。

* 如果浏览器本身不支持压缩功能，则返回选择的图片文件。

* 使用详见 index.html 里面的例子

------
###压缩结果

Android 4.3  Chrome/ 35.0.1916.141  quality 0.5  scale 720 :  原图 2250084 (2.14M) --> 压缩后 165751 (162K) 

Android 4.3 原生浏览器 不支持quality  scale 720 :  原图 2250084 (2.14M) --> 压缩后 629293 (614K)

Android 4.3 UC浏览器 不支持quality  scale 720 :  原图 2250084 (2.14M) --> 压缩后 692969 (676K)

iPad OS 7_0_4 Safari  图片太大时不支持quality scale 720: 原图 3193020 (3M) --> 压缩后 125255(122K)

iPone OS 7_1_2 Safari  图片太大时不支持quality scale 720: 原图 2010752 (1.92M) --> 压缩后 125255(199K)

