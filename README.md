###百度地图API 自定义标注图标

```js
var myIcon = new BMap.Icon("http://7xic1p.com1.z0.glb.clouddn.com/markers.png", new BMap.Size(23, 25), {
	offset: new BMap.Size(10, 25),
	imageOffset: new BMap.Size(0, 0 - i * 25) // 设置图片偏移  
});
var point = new BMap.Point(x,y);
// 创建标注对象并添加到地图 
var marker = new BMap.Marker(point,{icon: myIcon});
map.addOverlay(marker);
```

演示地址：http://itmyhome.com/baidu_map_icon