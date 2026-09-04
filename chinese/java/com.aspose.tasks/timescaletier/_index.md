---
title: "TimescaleTier"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示甘特图上时间尺度的单个层级。"
type: docs
weight: 325
url: /zh/java/com.aspose.tasks/timescaletier/
---

**Inheritance:**
java.lang.Object
```
public final class TimescaleTier
```

表示甘特图上时间尺度的单个层级。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [TimescaleTier()](#TimescaleTier--) | 初始化 [TimescaleTier](../../com.aspose.tasks/timescaletier) 类的新实例。 |
| [TimescaleTier(int unit, int count)](#TimescaleTier-int-int-) | 初始化 [TimescaleTier](../../com.aspose.tasks/timescaletier) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getAlignment()](#getAlignment--) | 获取在层级的每个时间段内对齐标签的方式（[HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)）。 |
| [getCount()](#getCount--) | 获取在该层级中显示标签的时间单位间隔。 |
| [getDateTimeConverter()](#getDateTimeConverter--) | 获取用于处理在此层级中渲染日期刻度的回调函数。 |
| [getLabel()](#getLabel--) | 获取时间刻度层级的日期标签 [DateLabel](../../com.aspose.tasks/datelabel)。 |
| [getRenderLabelOnEachPage()](#getRenderLabelOnEachPage--) | 获取标志，定义当时间段跨越多页时是否在每页渲染日期标签。 |
| [getShowTicks()](#getShowTicks--) | 获取指示是否在层级中显示分隔时间段的刻度线的值。 |
| [getUnit()](#getUnit--) | 获取时间刻度层级的时间刻度单位 [TimescaleUnit](../../com.aspose.tasks/timescaleunit)。 |
| [getUsesFiscalYear()](#getUsesFiscalYear--) | 获取指示是否基于财政年度来确定层级标签的值。 |
| [setAlignment(int value)](#setAlignment-int-) | 设置在层级的每个时间段内对齐标签的方式（[HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)）。 |
| [setCount(int value)](#setCount-int-) | 设置在该层级中显示标签的时间单位间隔。 |
| [setDateTimeConverter(DateTimeConverter value)](#setDateTimeConverter-com.aspose.tasks.DateTimeConverter-) | 设置用于处理在此层级中渲染日期刻度的回调函数。 |
| [setLabel(int value)](#setLabel-int-) | 设置时间刻度层级的日期标签 [DateLabel](../../com.aspose.tasks/datelabel)。 |
| [setRenderLabelOnEachPage(boolean value)](#setRenderLabelOnEachPage-boolean-) | 设置标志，定义当时间段跨越多页时是否在每页渲染日期标签。 |
| [setShowTicks(boolean value)](#setShowTicks-boolean-) | 设置指示是否在层级中显示分隔时间段的刻度线的值。 |
| [setUnit(int value)](#setUnit-int-) | 设置时间刻度层级的时间刻度单位 [TimescaleUnit](../../com.aspose.tasks/timescaleunit)。 |
| [setUsesFiscalYear(boolean value)](#setUsesFiscalYear-boolean-) | 设置指示是否基于财政年度来确定层级标签的值。 |
### TimescaleTier() {#TimescaleTier--}
```
public TimescaleTier()
```


初始化 [TimescaleTier](../../com.aspose.tasks/timescaletier) 类的新实例。

### TimescaleTier(int unit, int count) {#TimescaleTier-int-int-}
```
public TimescaleTier(int unit, int count)
```


初始化 [TimescaleTier](../../com.aspose.tasks/timescaletier) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| unit | int | 时间刻度单位 [TimescaleUnit](../../com.aspose.tasks/timescaleunit)。 |
| count | int | [TimescaleUnit](../../com.aspose.tasks/timescaleunit) 单位的计数。 |

### getAlignment() {#getAlignment--}
```
public final int getAlignment()
```


获取在层级的每个时间段内对齐标签的方式（[HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)）。

**Returns:**
int - 在层级的每个时间段内对齐标签的方式（[HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)）。
### getCount() {#getCount--}
```
public final int getCount()
```


获取在该层级中显示标签的时间单位间隔。默认值为 1。

**Returns:**
int - 在该层级中显示标签的时间单位间隔。
### getDateTimeConverter() {#getDateTimeConverter--}
```
public final DateTimeConverter getDateTimeConverter()
```


获取用于处理在此层级中渲染日期刻度的回调函数。

**Returns:**
[DateTimeConverter](../../com.aspose.tasks/datetimeconverter) - a callback function for handling rendering date tick in this tier.
### getLabel() {#getLabel--}
```
public final int getLabel()
```


获取时间刻度层级的日期标签 [DateLabel](../../com.aspose.tasks/datelabel)。

**Returns:**
int - 时间刻度层级的日期标签 [DateLabel](../../com.aspose.tasks/datelabel)。
### getRenderLabelOnEachPage() {#getRenderLabelOnEachPage--}
```
public final boolean getRenderLabelOnEachPage()
```


获取标志，定义当时间段跨越多页时是否在每页渲染日期标签。如果值为 'true'，当时间段跨越多页时，该期间的日期标签将在每页渲染。如果值为 'false'，日期标签仅根据 `Alignment`（[getAlignment](../../com.aspose.tasks/timescaletier\#getAlignment--)/[setAlignment(int)](../../com.aspose.tasks/timescaletier\#setAlignment-int-)) 属性的值渲染一次。

--------------------

在 MS Project 中没有对应的功能。

**Returns:**
boolean - 标志，定义当时间段跨越多个页面时是否在每页上渲染日期标签。
### getShowTicks() {#getShowTicks--}
```
public final boolean getShowTicks()
```


获取指示是否在层级中显示分隔时间段的刻度线的值。

**Returns:**
boolean - 表示是否在层级中显示分隔时间段的刻度线的值。
### getUnit() {#getUnit--}
```
public final int getUnit()
```


获取时间刻度层级的时间刻度单位 [TimescaleUnit](../../com.aspose.tasks/timescaleunit)。默认值为 [TimescaleUnit](../../com.aspose.tasks/timescaleunit)。

**Returns:**
int - 时间刻度层级的时间刻度单位 [TimescaleUnit](../../com.aspose.tasks/timescaleunit)。
### getUsesFiscalYear() {#getUsesFiscalYear--}
```
public final boolean getUsesFiscalYear()
```


获取指示是否基于财政年度来确定层级标签的值。

**Returns:**
boolean - 表示是否基于财政年度来确定层级标签的值。
### setAlignment(int value) {#setAlignment-int-}
```
public final void setAlignment(int value)
```


设置在层级的每个时间段内对齐标签的方式（[HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | int | 如何在层级的每个时间段内对齐标签（[HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)）。 |

### setCount(int value) {#setCount-int-}
```
public final void setCount(int value)
```


设置在层级中显示标签的时间单位间隔。默认值为 1。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 在层级中显示标签的时间单位间隔。 |

### setDateTimeConverter(DateTimeConverter value) {#setDateTimeConverter-com.aspose.tasks.DateTimeConverter-}
```
public final void setDateTimeConverter(DateTimeConverter value)
```


设置用于处理在此层级中渲染日期刻度的回调函数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [DateTimeConverter](../../com.aspose.tasks/datetimeconverter) | 用于在此层级中处理日期刻度渲染的回调函数。 |

### setLabel(int value) {#setLabel-int-}
```
public final void setLabel(int value)
```


设置时间刻度层级的日期标签 [DateLabel](../../com.aspose.tasks/datelabel)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | int | 时间刻度层级的日期标签 [DateLabel](../../com.aspose.tasks/datelabel)。 |

### setRenderLabelOnEachPage(boolean value) {#setRenderLabelOnEachPage-boolean-}
```
public final void setRenderLabelOnEachPage(boolean value)
```


设置标志，定义当时间段跨越多个页面时是否在每页上渲染日期标签。如果值为 'true'，当时间段跨越多个页面时，期间的日期标签会在每页上渲染。如果值为 'false'，日期标签仅根据 `Alignment`([getAlignment](../../com.aspose.tasks/timescaletier\#getAlignment--)/[setAlignment(int)](../../com.aspose.tasks/timescaletier\#setAlignment-int-)) 属性的值渲染一次。

--------------------

在 MS Project 中没有对应的功能。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 标志，定义当时间段跨越多个页面时是否在每页上渲染日期标签。 |

### setShowTicks(boolean value) {#setShowTicks-boolean-}
```
public final void setShowTicks(boolean value)
```


设置指示是否在层级中显示分隔时间段的刻度线的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 表示是否在层级中显示分隔时间段的刻度线的值。 |

### setUnit(int value) {#setUnit-int-}
```
public final void setUnit(int value)
```


设置时间刻度层级的时间刻度单位 [TimescaleUnit](../../com.aspose.tasks/timescaleunit)。默认值为 [TimescaleUnit](../../com.aspose.tasks/timescaleunit)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | int | 时间刻度层级的时间刻度单位 [TimescaleUnit](../../com.aspose.tasks/timescaleunit)。 |

### setUsesFiscalYear(boolean value) {#setUsesFiscalYear-boolean-}
```
public final void setUsesFiscalYear(boolean value)
```


设置指示是否基于财政年度来确定层级标签的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 表示是否基于财政年度来确定层级标签的值。 |

