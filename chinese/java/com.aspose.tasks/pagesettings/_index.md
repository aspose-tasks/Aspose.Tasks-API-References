---
title: "PageSettings"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示项目视图页面的打印设置。"
type: docs
weight: 181
url: /zh/java/com.aspose.tasks/pagesettings/
---

**Inheritance:**
java.lang.Object
```
public class PageSettings
```

表示项目视图页面的打印设置。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [PageSettings()](#PageSettings--) | 初始化 [PageSettings](../../com.aspose.tasks/pagesettings) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getAdjustToPercentOfNormalSize()](#getAdjustToPercentOfNormalSize--) | 获取一个值，指示是否将打印调整为指定的百分比（`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) 的正常大小。 |
| [getFirstPageNumber()](#getFirstPageNumber--) | 获取用于打印的起始页码。 |
| [getPagesInHeight()](#getPagesInHeight--) | 获取要打印的垂直页数。 |
| [getPagesInWidth()](#getPagesInWidth--) | 获取要打印的水平页数。 |
| [getPaperSize()](#getPaperSize--) | 获取纸张尺寸。 |
| [getPaperSizeId()](#getPaperSizeId--) | 获取一个整数，表示 PrinterPaperSize 值之一或自定义页面尺寸 ID。 |
| [getPercentOfNormalSize()](#getPercentOfNormalSize--) | 获取用于调整打印的正常尺寸百分比。 |
| [isPortrait()](#isPortrait--) | 获取一个值，指示页面方向是否为纵向；如果页面方向为横向则返回 false。 |
| [setAdjustToPercentOfNormalSize(boolean value)](#setAdjustToPercentOfNormalSize-boolean-) | 设置一个值，指示是否将打印调整为指定的百分比（`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) 的正常大小。 |
| [setFirstPageNumber(short value)](#setFirstPageNumber-short-) | 设置用于打印的起始页码。 |
| [setPagesInHeight(int value)](#setPagesInHeight-int-) | 设置要打印的垂直页数。 |
| [setPagesInWidth(int value)](#setPagesInWidth-int-) | 设置要打印的水平页数。 |
| [setPaperSize(int value)](#setPaperSize-int-) | 设置纸张尺寸。 |
| [setPaperSizeId(int value)](#setPaperSizeId-int-) | 设置一个整数，表示 PrinterPaperSize 值之一或自定义页面尺寸 ID。 |
| [setPercentOfNormalSize(int value)](#setPercentOfNormalSize-int-) | 设置用于调整打印的正常尺寸百分比。 |
| [setPortrait(boolean value)](#setPortrait-boolean-) | 设置一个值，指示页面方向是否为纵向；如果页面方向为横向则返回 false。 |
### PageSettings() {#PageSettings--}
```
public PageSettings()
```


初始化 [PageSettings](../../com.aspose/tasks/pagesettings) 类的新实例。表示项目视图页面的打印设置。

### getAdjustToPercentOfNormalSize() {#getAdjustToPercentOfNormalSize--}
```
public final boolean getAdjustToPercentOfNormalSize()
```


获取一个值，指示是否将打印调整为指定的百分比（`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) 的正常大小。

--------------------

在项目以 HTML 格式呈现时无效。

**Returns:**
boolean - 指示是否将打印调整为指定的百分比（`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) 的正常大小的值。
### getFirstPageNumber() {#getFirstPageNumber--}
```
public final short getFirstPageNumber()
```


获取用于打印的起始页码。

**Returns:**
short - 用于打印的起始页码。
### getPagesInHeight() {#getPagesInHeight--}
```
public final int getPagesInHeight()
```


获取要打印的垂直页数。

**Returns:**
int - 要打印的垂直页数。
### getPagesInWidth() {#getPagesInWidth--}
```
public final int getPagesInWidth()
```


获取要打印的水平页数。

**Returns:**
int - 要打印的水平页数。
### getPaperSize() {#getPaperSize--}
```
public final int getPaperSize()
```


获取纸张尺寸。可以是 [PrinterPaperSize](../../com.aspose/tasks/printerpapersize) 枚举的值之一。

**Returns:**
int - 纸张尺寸。
### getPaperSizeId() {#getPaperSizeId--}
```
public final int getPaperSizeId()
```


获取一个整数，表示 PrinterPaperSize 值之一或自定义页面尺寸 ID。此值可用于从操作系统设置中获取 PaperSize（）。

**Returns:**
int - 一个整数，表示 PrinterPaperSize 值之一或自定义页面大小 ID。
### getPercentOfNormalSize() {#getPercentOfNormalSize--}
```
public final int getPercentOfNormalSize()
```


获取用于调整打印的正常尺寸百分比。

**Returns:**
int - 一个相对于正常尺寸的百分比，用于调整打印。
### isPortrait() {#isPortrait--}
```
public final boolean isPortrait()
```


获取一个值，指示页面方向是否为纵向；如果页面方向为横向则返回 false。

--------------------

在渲染期间，当 SaveOptions.getPageSize() == PageSize.DefinedInView 时适用。

**Returns:**
boolean - 一个值，指示页面方向是否为纵向；如果页面方向为横向则返回 false。
### setAdjustToPercentOfNormalSize(boolean value) {#setAdjustToPercentOfNormalSize-boolean-}
```
public final void setAdjustToPercentOfNormalSize(boolean value)
```


设置一个值，指示是否将打印调整为指定的百分比（`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) 的正常大小。

--------------------

在项目以 HTML 格式呈现时无效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | boolean | 一个值，指示是否将打印调整为指定的百分比（`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose.tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose.tasks/pagesettings\#setPercentOfNormalSize-int-))）的正常尺寸。 |

### setFirstPageNumber(short value) {#setFirstPageNumber-short-}
```
public final void setFirstPageNumber(short value)
```


设置用于打印的起始页码。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | short | 用于打印的起始页码。 |

### setPagesInHeight(int value) {#setPagesInHeight-int-}
```
public final void setPagesInHeight(int value)
```


设置要打印的垂直页数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 要打印的高度页数。 |

### setPagesInWidth(int value) {#setPagesInWidth-int-}
```
public final void setPagesInWidth(int value)
```


设置要打印的水平页数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 要打印的宽度页数。 |

### setPaperSize(int value) {#setPaperSize-int-}
```
public final void setPaperSize(int value)
```


设置纸张大小。可以是 [PrinterPaperSize](../../com.aspose.tasks/printerpapersize) 枚举的值之一。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 纸张大小。 |

### setPaperSizeId(int value) {#setPaperSizeId-int-}
```
public final void setPaperSizeId(int value)
```


设置一个整数，表示 PrinterPaperSize 值之一或自定义页面大小 ID。此值可用于从操作系统设置中获取 PaperSize（）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 一个整数，表示 PrinterPaperSize 值之一或自定义页面大小 ID。 |

### setPercentOfNormalSize(int value) {#setPercentOfNormalSize-int-}
```
public final void setPercentOfNormalSize(int value)
```


设置用于调整打印的正常尺寸百分比。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 用于调整打印的正常尺寸百分比。 |

### setPortrait(boolean value) {#setPortrait-boolean-}
```
public final void setPortrait(boolean value)
```


设置一个值，指示页面方向是否为纵向；如果页面方向为横向则返回 false。

--------------------

在渲染期间，当 SaveOptions.getPageSize() == PageSize.DefinedInView 时适用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个值，指示页面方向是否为纵向；如果页面方向为横向则返回 false。 |

