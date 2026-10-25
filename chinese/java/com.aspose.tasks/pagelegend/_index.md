---
title: "PageLegend"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示用于项目打印的页面图例。"
type: docs
weight: 177
url: /zh/java/com.aspose.tasks/pagelegend/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.HeaderFooterInfo](../../com.aspose.tasks/headerfooterinfo)
```
public class PageLegend extends HeaderFooterInfo
```

表示用于项目打印的页面图例。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [PageLegend()](#PageLegend--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getLegendOn()](#getLegendOn--) | 获取图例出现的页面。 |
| [getWidth()](#getWidth--) | 获取图例左侧部分（默认包含项目名称和日期）的宽度（单位：厘米）。 |
| [setLegendOn(int value)](#setLegendOn-int-) | 设置图例出现的页面。 |
| [setWidth(double value)](#setWidth-double-) | 设置图例左侧部分（默认包含项目名称和日期）的宽度（单位：厘米）。 |
### PageLegend() {#PageLegend--}
```
public PageLegend()
```


### getLegendOn() {#getLegendOn--}
```
public final int getLegendOn()
```


获取图例出现的页面。可以是 [Legend](../../com.aspose/tasks/legend) 枚举的其中一个值。

**Returns:**
int - 图例出现的页面。
### getWidth() {#getWidth--}
```
public final double getWidth()
```


获取图例左侧部分（默认包含项目名称和日期）的宽度（单位：厘米）。

**Returns:**
double - 图例左侧部分的宽度（默认包含项目名称和日期），单位为厘米。
### setLegendOn(int value) {#setLegendOn-int-}
```
public final void setLegendOn(int value)
```


设置图例出现的页面。可以是 [Legend](../../com.aspose.tasks/legend) 枚举的其中一个值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 图例出现的页面。 |

### setWidth(double value) {#setWidth-double-}
```
public final void setWidth(double value)
```


设置图例左侧部分（默认包含项目名称和日期）的宽度（单位：厘米）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double | 图例左侧部分的宽度（默认包含项目名称和日期），单位为厘米。 |

