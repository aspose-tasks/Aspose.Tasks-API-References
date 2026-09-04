---
title: "ImageFormat"
second_title: "Aspose.Tasks for Java API 参考"
description: "指定图像的文件格式。"
type: docs
weight: 133
url: /zh/java/com.aspose.tasks/imageformat/
---

**Inheritance:**
java.lang.Object
```
public final class ImageFormat
```

指定图像的文件格式。不能被扩展。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ImageFormat(String guid)](#ImageFormat-java.lang.String-) | 使用指定的 Guid 字符串初始化 ImageFormat 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object o)](#equals-java.lang.Object-) | 返回一个值，指示指定的对象是否为等同于此 ImageFormat 对象的 ImageFormat 对象。 |
| [getBmp()](#getBmp--) | 获取位图 (BMP) 图像格式。 |
| [getEmf()](#getEmf--) | 获取增强型元文件 (EMF) 图像格式。 |
| [getExif()](#getExif--) | 获取可交换图像文件 (Exif) 格式。 |
| [getGif()](#getGif--) | 获取图形交换格式 (GIF) 图像格式。 |
| [getGuid()](#getGuid--) | 获取表示此 ImageFormat 对象的 Guid 字符串。 |
| [getIcon()](#getIcon--) | 获取 Windows 图标图像格式。 |
| [getJpeg()](#getJpeg--) | 获取联合图像专家组 (JPEG) 图像格式。 |
| [getMemoryBmp()](#getMemoryBmp--) | 获取内存中位图的格式。 |
| [getPng()](#getPng--) | 获取 W3C 可移植网络图形 (PNG) 图像格式。 |
| [getTiff()](#getTiff--) | 获取标记图像文件格式 (TIFF) 图像格式。 |
| [getWmf()](#getWmf--) | 获取 Windows 元文件 (WMF) 图像格式。 |
| [hashCode()](#hashCode--) | 返回表示此对象的哈希码值。 |
| [isBitmapType()](#isBitmapType--) | 确定图像格式是否为位图类型。 |
| [isMetafileType()](#isMetafileType--) | 确定图像格式是否为元文件类型。 |
| [isUnknownType()](#isUnknownType--) | 确定图像格式是否为未知类型。 |
| [toString()](#toString--) | 将此 ImageFormat 对象转换为可读的字符串。 |
### ImageFormat(String guid) {#ImageFormat-java.lang.String-}
```
public ImageFormat(String guid)
```


使用指定的 Guid 字符串初始化 ImageFormat 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| guid | java.lang.String | 指定特定图像格式的 Guid 字符串。 |

### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```


返回一个值，指示指定的对象是否为等同于此 ImageFormat 对象的 ImageFormat 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | 要测试的对象。 |

**Returns:**
boolean - 如果 o 是与此 ImageFormat 对象等价的 ImageFormat 对象，则为 true；否则为 false。
### getBmp() {#getBmp--}
```
public static ImageFormat getBmp()
```


获取位图 (BMP) 图像格式。

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the bitmap image format.
### getEmf() {#getEmf--}
```
public static ImageFormat getEmf()
```


获取增强型元文件 (EMF) 图像格式。

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the enhanced metafile image format.
### getExif() {#getExif--}
```
public static ImageFormat getExif()
```


获取可交换图像文件 (Exif) 格式。

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the Exif format.
### getGif() {#getGif--}
```
public static ImageFormat getGif()
```


获取图形交换格式 (GIF) 图像格式。

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the GIF image format.
### getGuid() {#getGuid--}
```
public String getGuid()
```


获取表示此 ImageFormat 对象的 Guid 字符串。

**Returns:**
java.lang.String - 表示此 ImageFormat 对象的 Guid 字符串。
### getIcon() {#getIcon--}
```
public static ImageFormat getIcon()
```


获取 Windows 图标图像格式。

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the Windows icon image format.
### getJpeg() {#getJpeg--}
```
public static ImageFormat getJpeg()
```


获取联合图像专家组 (JPEG) 图像格式。

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the JPEG image format.
### getMemoryBmp() {#getMemoryBmp--}
```
public static ImageFormat getMemoryBmp()
```


获取内存中位图的格式。

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the format of a bitmap in memory.
### getPng() {#getPng--}
```
public static ImageFormat getPng()
```


获取 W3C 可移植网络图形 (PNG) 图像格式。

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the PNG image format.
### getTiff() {#getTiff--}
```
public static ImageFormat getTiff()
```


获取标记图像文件格式 (TIFF) 图像格式。

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the TIFF image format.
### getWmf() {#getWmf--}
```
public static ImageFormat getWmf()
```


获取 Windows 元文件 (WMF) 图像格式。

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the Windows metafile image format.
### hashCode() {#hashCode--}
```
public int hashCode()
```


返回表示此对象的哈希码值。

**Returns:**
int - 表示此对象的哈希码。
### isBitmapType() {#isBitmapType--}
```
public boolean isBitmapType()
```


确定图像格式是否为位图类型。

**Returns:**
boolean - 如果图像格式是位图类型，则为 true；否则为 false。
### isMetafileType() {#isMetafileType--}
```
public boolean isMetafileType()
```


确定图像格式是否为元文件类型。

**Returns:**
boolean - 如果图像格式是元文件类型，则为 true；否则为 false。
### isUnknownType() {#isUnknownType--}
```
public boolean isUnknownType()
```


确定图像格式是否为未知类型。

**Returns:**
boolean - 如果图像格式是未知类型，则为 true；否则为 false。
### toString() {#toString--}
```
public String toString()
```


将此 ImageFormat 对象转换为可读的字符串。

**Returns:**
java.lang.String - 表示此 ImageFormat 对象的字符串。
