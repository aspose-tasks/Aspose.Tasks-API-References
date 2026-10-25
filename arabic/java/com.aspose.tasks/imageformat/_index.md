---
title: "ImageFormat"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يحدد تنسيق ملف الصورة."
type: docs
weight: 133
url: /ar/java/com.aspose.tasks/imageformat/
---

**Inheritance:**
java.lang.Object
```
public final class ImageFormat
```

يحدد تنسيق ملف الصورة. لا يمكن توسيعه.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [ImageFormat(String guid)](#ImageFormat-java.lang.String-) | ينشئ مثيلاً جديدًا من فئة ImageFormat باستخدام سلسلة Guid المحددة. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object o)](#equals-java.lang.Object-) | يعيد قيمة تشير إلى ما إذا كان الكائن المحدد هو كائن ImageFormat مكافئ لهذا الكائن ImageFormat. |
| [getBmp()](#getBmp--) | يحصل على تنسيق صورة bitmap (BMP). |
| [getEmf()](#getEmf--) | يحصل على تنسيق صورة enhanced metafile (EMF). |
| [getExif()](#getExif--) | يحصل على تنسيق Exchangeable Image File (Exif). |
| [getGif()](#getGif--) | يحصل على تنسيق صورة Graphics Interchange Format (GIF). |
| [getGuid()](#getGuid--) | يحصل على سلسلة Guid تمثل كائن ImageFormat هذا. |
| [getIcon()](#getIcon--) | يحصل على تنسيق صورة أيقونة Windows. |
| [getJpeg()](#getJpeg--) | يحصل على تنسيق صورة Joint Photographic Experts Group (JPEG). |
| [getMemoryBmp()](#getMemoryBmp--) | يحصل على تنسيق bitmap في الذاكرة. |
| [getPng()](#getPng--) | يحصل على تنسيق صورة W3C Portable Network Graphics (PNG). |
| [getTiff()](#getTiff--) | يحصل على تنسيق صورة Tagged Image File Format (TIFF). |
| [getWmf()](#getWmf--) | يحصل على تنسيق صورة Windows metafile (WMF). |
| [hashCode()](#hashCode--) | يعيد قيمة رمز تجزئة تمثل هذا الكائن. |
| [isBitmapType()](#isBitmapType--) | يحدد ما إذا كان تنسيق الصورة من نوع bitmap. |
| [isMetafileType()](#isMetafileType--) | يحدد ما إذا كان تنسيق الصورة من نوع metafile. |
| [isUnknownType()](#isUnknownType--) | يحدد ما إذا كان تنسيق الصورة من نوع غير معروف. |
| [toString()](#toString--) | يحوّل كائن ImageFormat هذا إلى سلسلة قابلة للقراءة من قبل الإنسان. |
### ImageFormat(String guid) {#ImageFormat-java.lang.String-}
```
public ImageFormat(String guid)
```


ينشئ مثيلاً جديدًا من فئة ImageFormat باستخدام سلسلة Guid المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| guid | java.lang.String | سلسلة Guid التي تحدد تنسيق صورة معين. |

### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```


يعيد قيمة تشير إلى ما إذا كان الكائن المحدد هو كائن ImageFormat مكافئ لهذا الكائن ImageFormat.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | الكائن المراد اختباره. |

**Returns:**
منطقي - true إذا كان o كائن ImageFormat يساوي هذا الكائن ImageFormat؛ وإلا، false.
### getBmp() {#getBmp--}
```
public static ImageFormat getBmp()
```


يحصل على تنسيق صورة bitmap (BMP).

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the bitmap image format.
### getEmf() {#getEmf--}
```
public static ImageFormat getEmf()
```


يحصل على تنسيق صورة enhanced metafile (EMF).

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the enhanced metafile image format.
### getExif() {#getExif--}
```
public static ImageFormat getExif()
```


يحصل على تنسيق Exchangeable Image File (Exif).

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the Exif format.
### getGif() {#getGif--}
```
public static ImageFormat getGif()
```


يحصل على تنسيق صورة Graphics Interchange Format (GIF).

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the GIF image format.
### getGuid() {#getGuid--}
```
public String getGuid()
```


يحصل على سلسلة Guid تمثل كائن ImageFormat هذا.

**Returns:**
java.lang.String - سلسلة Guid تمثل هذا الكائن ImageFormat.
### getIcon() {#getIcon--}
```
public static ImageFormat getIcon()
```


يحصل على تنسيق صورة أيقونة Windows.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the Windows icon image format.
### getJpeg() {#getJpeg--}
```
public static ImageFormat getJpeg()
```


يحصل على تنسيق صورة Joint Photographic Experts Group (JPEG).

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the JPEG image format.
### getMemoryBmp() {#getMemoryBmp--}
```
public static ImageFormat getMemoryBmp()
```


يحصل على تنسيق bitmap في الذاكرة.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the format of a bitmap in memory.
### getPng() {#getPng--}
```
public static ImageFormat getPng()
```


يحصل على تنسيق صورة W3C Portable Network Graphics (PNG).

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the PNG image format.
### getTiff() {#getTiff--}
```
public static ImageFormat getTiff()
```


يحصل على تنسيق صورة Tagged Image File Format (TIFF).

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the TIFF image format.
### getWmf() {#getWmf--}
```
public static ImageFormat getWmf()
```


يحصل على تنسيق صورة Windows metafile (WMF).

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the Windows metafile image format.
### hashCode() {#hashCode--}
```
public int hashCode()
```


يعيد قيمة رمز تجزئة تمثل هذا الكائن.

**Returns:**
int - رمز تجزئة يمثل هذا الكائن.
### isBitmapType() {#isBitmapType--}
```
public boolean isBitmapType()
```


يحدد ما إذا كان تنسيق الصورة من نوع bitmap.

**Returns:**
منطقي - true إذا كان تنسيق الصورة من نوع bitmap؛ وإلا، false.
### isMetafileType() {#isMetafileType--}
```
public boolean isMetafileType()
```


يحدد ما إذا كان تنسيق الصورة من نوع metafile.

**Returns:**
منطقي - true إذا كان تنسيق الصورة من نوع metafile؛ وإلا، false.
### isUnknownType() {#isUnknownType--}
```
public boolean isUnknownType()
```


يحدد ما إذا كان تنسيق الصورة من نوع غير معروف.

**Returns:**
منطقي - true إذا كان تنسيق الصورة من نوع غير معروف؛ وإلا، false.
### toString() {#toString--}
```
public String toString()
```


يحوّل كائن ImageFormat هذا إلى سلسلة قابلة للقراءة من قبل الإنسان.

**Returns:**
java.lang.String - سلسلة تمثل هذا الكائن ImageFormat.
