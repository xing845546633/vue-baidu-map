# 基础

## 常量

### ControlAnchor

此常量表示控件的定位。

|常量|描述|
|----|----|
|BMAP_ANCHOR_TOP_LEFT|控件将定位到地图的左上角|
|BMAP_ANCHOR_TOP_RIGHT|控件将定位到地图的右上角|
|BMAP_ANCHOR_BOTTOM_LEFT|控件将定位到地图的左下角|
|BMAP_ANCHOR_BOTTOM_RIGHT|控件将定位到地图的右下角|

### NavigationControlType

此常量表示平移缩放控件的类型。

|常量|描述|
|----|----|
|BMAP_NAVIGATION_CONTROL_LARGE|标准的平移缩放控件（包括平移、缩放按钮和滑块）|
|BMAP_NAVIGATION_CONTROL_SMALL|仅包含平移和缩放按钮|
|BMAP_NAVIGATION_CONTROL_PAN|仅包含平移按钮|
|BMAP_NAVIGATION_CONTROL_ZOOM|仅包含缩放按钮|

### MapTypeControlType

此常量表示MapTypeControl的外观样式。

|常量|描述|
|----|----|
|BMAP_MAPTYPE_CONTROL_HORIZONTAL|按钮水平方式展示，默认采用此类型展示|
|BMAP_MAPTYPE_CONTROL_DROPDOWN|按钮呈下拉列表方式展示|
|BMAP_MAPTYPE_CONTROL_MAP|以图片方式展示类型控件，设置该类型后无法指定maptypes属性|

### Animation

此常量表示标注的动画效果。

|常量|描述|
|----|----|
|BMAP_ANIMATION_DROP|坠落动画|
|BMAP_ANIMATION_BOUNCE|跳动动画|

### MapType

表示一种地图类型。

|常量|描述|
|----|----|
|BMAP_NORMAL_MAP|此地图类型展示普通街道视图|
|BMAP_PERSPECTIVE_MAP|此地图类型展示透视图像视图|
|BMAP_SATELLITE_MAP|此地图类型展示卫星视图|
|BMAP_HYBRID_MAP|此地图类型展示卫星和路网的混合视图|

### LengthUnit

常量表示长度单位制。

|常量|描述|
|----|----|
|BMAP_UNIT_METRIC|公制单位|
|BMAP_UNIT_IMPERIAL|英制单位|

### HighlightModes

此常量用于描述对象当前状态。

|常量|描述|
|----|----|
|BMAP_HIGHLIGHT_STEP|驾车结果展现中点击列表后的展现点步骤|
|BMAP_HIGHLIGHT_ROUTE|驾车结果展现中点击列表后的展现路段|



## 私有类型

### Point

用于描述地图上点的经纬度。

#### 结构

```javascript
{
  lng: Number
  lat: Number
}
```

### Size

用于描述地图上制定区域的长宽尺寸。

#### 结构

```javascript
{
  width: Number,
  height: Number
}
```

### Pixel

用于描述地图上某一个像素点的坐标。

#### 结构

```javascript
{
  x: Number,
  y: Number
}
```

### Bounds

用于描述地图上的一片区域上由西南和东北两个坐标围成的一片区域。

#### 结构

```javascript
{
  sw: Number,
  ne: Number
}
```

### Icon

声明一个图标。

#### 结构

```javascript
{
  url: String,
  size: Size,
  opts: {
    anchor: Size,
    imageOffset: Size,
    infoWindowAnchor: Size,
    printImageUrl: String
  }
}
```

### Label

声明一个标签。

```javascript
{
  content: String,
  opts: {
    offset: Size
    position: Point,
    enableMassClear: Boolean
  }
}
```

## 参考

> [百度地图官方文档](http://lbsyun.baidu.com/cms/jsapi/reference/jsapi_reference.html)