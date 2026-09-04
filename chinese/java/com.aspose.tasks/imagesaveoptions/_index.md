---
title: "ImageSaveOptions"
second_title: "Aspose.Tasks for Java API 参考"
description: "允许在将项目页面渲染为图像时指定其他选项。"
type: docs
weight: 134
url: /zh/java/com.aspose.tasks/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class ImageSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

允许在将项目页面渲染为图像时指定其他选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ImageSaveOptions(int saveFormat)](#ImageSaveOptions-int-) | 初始化 [ImageSaveOptions](../../com.aspose.tasks/imagesaveoptions) 类的新实例，可用于将渲染的图像保存为 TIFF、PNG、BMP 或 JPEG 格式。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getFontSettings()](#getFontSettings--) | 指定在渲染项目视图时使用的字体设置。 |
| [getHorizontalResolution()](#getHorizontalResolution--) | 获取水平分辨率（dpi）。 |
| [getJpegQuality()](#getJpegQuality--) | 获取 JPEG 质量。 |
| [getPageSavingCallback()](#getPageSavingCallback--) | 获取用户定义的回调，用于为每个渲染的页面获取输出流。 |
| [getPages()](#getPages--) | 获取在将项目布局保存为单独文件时要保存的页码列表。 |
| [getPixelFormat()](#getPixelFormat--) | 获取图像中每个像素的颜色数据格式。 |
| [getReduceFooterGap()](#getReduceFooterGap--) | 获取指示是否必须缩小最后任务与页脚之间间距的值。 |
| [getTiffCompression()](#getTiffCompression--) | 获取将生成的图像保存为 TIFF 格式时使用的压缩类型。 |
| [getVerticalResolution()](#getVerticalResolution--) | 获取垂直分辨率（dpi）。 |
| [setHorizontalResolution(float value)](#setHorizontalResolution-float-) | 设置水平分辨率（dpi）。 |
| [setJpegQuality(int value)](#setJpegQuality-int-) | 设置 JPEG 质量。 |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | 设置用户定义的回调函数，用于获取每个渲染页面的输出流。 |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | 设置在将项目布局保存为单独文件时要保存的页码列表。 |
| [setPixelFormat(int value)](#setPixelFormat-int-) | 设置图像中每个像素的颜色数据格式。 |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | 设置一个值，指示是否必须缩小最后任务与页脚之间的间距。 |
| [setTiffCompression(int value)](#setTiffCompression-int-) | 设置将生成的图像保存为 TIFF 格式时使用的压缩类型。 |
| [setVerticalResolution(float value)](#setVerticalResolution-float-) | 设置垂直分辨率（dpi）。 |
### ImageSaveOptions(int saveFormat) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int saveFormat)
```


初始化 [ImageSaveOptions](../../com.aspose.tasks/imagesaveoptions) 类的新实例，可用于将渲染的图像保存为 TIFF、PNG、BMP 或 JPEG 格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| saveFormat | int | 可以是 TIFF、PNG、BMP 或 JPEG[SaveFileFormat](../../com.aspose.tasks/savefileformat)。 |

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public final void copyOutputPropertiesFrom(SaveOptions source)
```


保留供内部使用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| source | [SaveOptions](../../com.aspose.tasks/saveoptions) | \{@inheritDoc\} |

### deepClone() {#deepClone--}
```
public SaveOptions deepClone()
```


保留供内部使用。

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


指定在渲染项目视图时使用的字体设置。

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getHorizontalResolution() {#getHorizontalResolution--}
```
public final float getHorizontalResolution()
```


获取水平分辨率（dpi）。

**Returns:**
float - 水平分辨率（dpi）。
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


获取 JPEG 质量。允许的取值范围是 0..100。

**Returns:**
int - JPEG 质量。
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


获取用户定义的回调，用于为每个渲染的页面获取输出流。

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


获取在将项目布局保存为单独文件时要保存的页码列表。

--------------------

如果此列表为空，将保存所有页面。

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - 在将项目布局保存为单独文件时要保存的页码列表。
### getPixelFormat() {#getPixelFormat--}
```
public final int getPixelFormat()
```


获取图像中每个像素的颜色数据格式。

**Returns:**
int - 图像中每个像素的颜色数据格式。
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


获取指示是否必须缩小最后任务与页脚之间间距的值。

**Returns:**
boolean - 一个值，指示是否必须缩小最后任务与页脚之间的间距。
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


获取将生成的图像保存为 TIFF 格式时使用的压缩类型。

--------------------

仅在保存为 TIFF 时有效。默认值为 `TiffCompressionLZW`([getTiffCompression()](../../com.aspose.tasks/imagesaveoptions\\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\\#setTiffCompression-int-))。

**Returns:**
int - 将生成的图像保存为 TIFF 格式时使用的压缩类型。
### getVerticalResolution() {#getVerticalResolution--}
```
public final float getVerticalResolution()
```


获取垂直分辨率（dpi）。

**Returns:**
float - 垂直分辨率（dpi）。
### setHorizontalResolution(float value) {#setHorizontalResolution-float-}
```
public final void setHorizontalResolution(float value)
```


设置水平分辨率（dpi）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | float | 水平分辨率（dpi）。 |

### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


设置 JPEG 质量。允许的取值范围是 0..100。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | JPEG 质量。 |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


设置用户定义的回调函数，用于获取每个渲染页面的输出流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | 用户定义的回调，用于获取每个渲染页面的输出流。 |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


设置在将项目布局保存为单独文件时要保存的页码列表。

--------------------

如果此列表为空，将保存所有页面。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.List&lt;java.lang.Integer&gt; | 在将项目布局保存为单独文件时要保存的页码列表。 |

### setPixelFormat(int value) {#setPixelFormat-int-}
```
public final void setPixelFormat(int value)
```


设置图像中每个像素的颜色数据格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 图像中每个像素的颜色数据格式。 |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


设置一个值，指示是否必须缩小最后任务与页脚之间的间距。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示是否应缩小最后任务与页脚之间间距的值。 |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


设置将生成的图像保存为 TIFF 格式时使用的压缩类型。

--------------------

仅在保存为 TIFF 时有效。默认值为 `TiffCompressionLZW`([getTiffCompression()](../../com.aspose.tasks/imagesaveoptions\\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\\#setTiffCompression-int-))。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 将生成的图像保存为 TIFF 格式时使用的压缩类型。 |

### setVerticalResolution(float value) {#setVerticalResolution-float-}
```
public final void setVerticalResolution(float value)
```


设置垂直分辨率（dpi）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | float | 垂直分辨率（dpi）。 |

