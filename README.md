
##ios免越狱定位外挂，用于破解打卡软件

手把手教你做一个定位外挂，让你轻松在家实现上下班打卡。

* step1：创建一个ios项目名称随意。

* step2:   cmd+n 创建一个GPX文件 。
![创建GPX文件](http://i4.buimg.com/1949/e67d0e74bf3689f8.png)
* step3: 复制下面代码，替换gpx文件中的代码

```
<?xml version="1.0" encoding="UTF-8" ?>
<gpx version="1.1"
    creator="GMapToGPX 6.4j - http://www.elsewhere.org/GMapToGPX/"
    xmlns="http://www.topografix.com/GPX/1/1"
    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    xsi:schemaLocation="http://www.topografix.com/GPX/1/1 http://www.topografix.com/GPX/1/1/gpx.xsd">
    <wpt lat="39.981101" lon="116.449488">

    </wpt>
</gpx>
```

其中  `<wpt lat="39.981101" lon="116.449488">`  需要修改为你需要的坐标。

* step4: [点击这里查看你公司所在的坐标](http://lbs.amap.com/console/show/picker)。

* step5: 坐标替换完成后，在`Edit Scheme`的options中 修改`Default Location`为创建的gpx文件名称。

![配置gpx文件](http://i1.piimg.com/1949/56ff44266adb1e79.png)

或者

在 `Debug -> Simulate Loaction`中选中创建的gpx文件。
![配置gpx文件](http://i1.piimg.com/1949/d93901a780fb3e8c.png) 

* step6:运行项目即可。运行成功后，您的手机的位置将一直定位在目标坐标，包括高德地图、百度地图、钉钉、微信。如需展示正常的位置还需杀死项目进程，重启手机。（如有好的解决方法，还请指教）。



 