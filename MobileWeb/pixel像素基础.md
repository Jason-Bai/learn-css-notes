## pixel像素基础

iphone 5 640*1136（物理像素）

px: CSS pixel 逻辑像素，浏览器使用的抽象单位

dp,pt: device independent pixels 设备无关像素

dpr: devicePixelRatio 设备像素缩放比

1px = dpr * dpr * dp


---

DPI: 打印机每英寸可以喷的墨汁点（印刷行业）
PPI: 屏幕每英寸的像素数量，即单位英寸内的像素密度

已iphone 5为例:

PPI = ( 物理x * 物理x + 物理y * 物理y) / 4 = 326ppi（视网膜Retina屏）
