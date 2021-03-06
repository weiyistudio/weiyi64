# weiyi64
OpenCV基于浏览器的在线车牌识别系统的设计与实现

#### 介绍
针对目前发现的问题，本课题在分析了当前车牌识别技术的应用范围以及对此技术未覆盖的区域进行分析比较的基础上，针对未覆盖区域，扩大此技术的服务范围，设计研发了基于浏览器的车牌识别系统。本系统的主要分为解码部分，识别部分和消息传递部分。在解码部分使用ffmpge对用户上传的视频进行处理，将上传的视频流截取成RGB格式的图片储存；识别部分使用OpenCV技术，对RGB格式图片进行降噪，车牌定位，边缘识别，字符识别处理；消息传递部分使用rabbitMQ技术，将解码部分和识别部分与浏览器前台操作结合，并在识别结束后将识别信息传回浏览器页面显示。

![输入图片说明](https://images.gitee.com/uploads/images/2020/1129/223304_213a9463_4865385.png "屏幕截图.png")

车牌识别系统主要分为客户层应用层和数据层。客户在浏览器端发出Start请求，消息经过处理后传递至应用层。在应用层对客户上传的视频进行提取分帧，对分帧图像进行置灰、二值化、校正、分割和识别处理处理，处理消息传回浏览器显示，图像信息暂时保留在数据层，识别完成后删除信息。

![输入图片说明](https://images.gitee.com/uploads/images/2020/1129/223321_c3fc4dbe_4865385.png "屏幕截图.png")

![输入图片说明](https://images.gitee.com/uploads/images/2020/1129/223336_9bfab99e_4865385.png "屏幕截图.png")


联系Q：2762501186
![输入图片说明](https://images.gitee.com/uploads/images/2020/1119/003728_cd598bb9_4865385.jpeg "微信.jpg")
