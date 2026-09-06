---
title: "ImageFormat"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Resmin dosya biçimini belirtir."
type: docs
weight: 133
url: /tr/java/com.aspose.tasks/imageformat/
---

**Inheritance:**
java.lang.Object
```
public final class ImageFormat
```

Görselin dosya formatını belirtir. Genişletilemez.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ImageFormat(String guid)](#ImageFormat-java.lang.String-) | Belirtilen Guid dizesini kullanarak ImageFormat sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object o)](#equals-java.lang.Object-) | Belirtilen nesnenin bu ImageFormat nesnesine eşdeğer bir ImageFormat nesnesi olup olmadığını gösteren bir değer döndürür. |
| [getBmp()](#getBmp--) | Bitmap (BMP) görüntü formatını alır. |
| [getEmf()](#getEmf--) | Gelişmiş metafile (EMF) görüntü formatını alır. |
| [getExif()](#getExif--) | Değiştirilebilir Görüntü Dosyası (Exif) formatını alır. |
| [getGif()](#getGif--) | Graphics Interchange Format (GIF) görüntü formatını alır. |
| [getGuid()](#getGuid--) | Bu ImageFormat nesnesini temsil eden bir Guid dizesi alır. |
| [getIcon()](#getIcon--) | Windows simge görüntü formatını alır. |
| [getJpeg()](#getJpeg--) | Joint Photographic Experts Group (JPEG) görüntü formatını alır. |
| [getMemoryBmp()](#getMemoryBmp--) | Bellekteki bir bitmap'in formatını alır. |
| [getPng()](#getPng--) | W3C Portable Network Graphics (PNG) görüntü formatını alır. |
| [getTiff()](#getTiff--) | Tagged Image File Format (TIFF) görüntü formatını alır. |
| [getWmf()](#getWmf--) | Windows metafile (WMF) görüntü formatını alır. |
| [hashCode()](#hashCode--) | Bu nesneyi temsil eden bir karma kod değeri döndürür. |
| [isBitmapType()](#isBitmapType--) | Bir görüntü formatının bitmap türü olup olmadığını belirler. |
| [isMetafileType()](#isMetafileType--) | Bir görüntü formatının metafile türü olup olmadığını belirler. |
| [isUnknownType()](#isUnknownType--) | Bir görüntü formatının bilinmeyen tür olup olmadığını belirler. |
| [toString()](#toString--) | Bu ImageFormat nesnesini okunabilir bir dizeye dönüştürür. |
### ImageFormat(String guid) {#ImageFormat-java.lang.String-}
```
public ImageFormat(String guid)
```


Belirtilen Guid dizesini kullanarak ImageFormat sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| guid | java.lang.String | Belirli bir görüntü formatını belirten Guid dizesi. |

### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```


Belirtilen nesnenin bu ImageFormat nesnesine eşdeğer bir ImageFormat nesnesi olup olmadığını gösteren bir değer döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| o | java.lang.Object | Test edilecek nesne. |

**Returns:**
boolean - true ise o, bu ImageFormat nesnesine eşdeğer bir ImageFormat nesnesidir; aksi takdirde false.
### getBmp() {#getBmp--}
```
public static ImageFormat getBmp()
```


Bitmap (BMP) görüntü formatını alır.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the bitmap image format.
### getEmf() {#getEmf--}
```
public static ImageFormat getEmf()
```


Gelişmiş metafile (EMF) görüntü formatını alır.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the enhanced metafile image format.
### getExif() {#getExif--}
```
public static ImageFormat getExif()
```


Değiştirilebilir Görüntü Dosyası (Exif) formatını alır.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the Exif format.
### getGif() {#getGif--}
```
public static ImageFormat getGif()
```


Graphics Interchange Format (GIF) görüntü formatını alır.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the GIF image format.
### getGuid() {#getGuid--}
```
public String getGuid()
```


Bu ImageFormat nesnesini temsil eden bir Guid dizesi alır.

**Returns:**
java.lang.String - Bu ImageFormat nesnesini temsil eden bir Guid dizesi.
### getIcon() {#getIcon--}
```
public static ImageFormat getIcon()
```


Windows simge görüntü formatını alır.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the Windows icon image format.
### getJpeg() {#getJpeg--}
```
public static ImageFormat getJpeg()
```


Joint Photographic Experts Group (JPEG) görüntü formatını alır.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the JPEG image format.
### getMemoryBmp() {#getMemoryBmp--}
```
public static ImageFormat getMemoryBmp()
```


Bellekteki bir bitmap'in formatını alır.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the format of a bitmap in memory.
### getPng() {#getPng--}
```
public static ImageFormat getPng()
```


W3C Portable Network Graphics (PNG) görüntü formatını alır.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the PNG image format.
### getTiff() {#getTiff--}
```
public static ImageFormat getTiff()
```


Tagged Image File Format (TIFF) görüntü formatını alır.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the TIFF image format.
### getWmf() {#getWmf--}
```
public static ImageFormat getWmf()
```


Windows metafile (WMF) görüntü formatını alır.

**Returns:**
[ImageFormat](../../com.aspose.tasks/imageformat) - An ImageFormat object that indicates the Windows metafile image format.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Bu nesneyi temsil eden bir karma kod değeri döndürür.

**Returns:**
int - Bu nesneyi temsil eden bir karma kodu.
### isBitmapType() {#isBitmapType--}
```
public boolean isBitmapType()
```


Bir görüntü formatının bitmap türü olup olmadığını belirler.

**Returns:**
boolean - true ise bir görüntü biçimi bitmap türündedir; aksi takdirde false.
### isMetafileType() {#isMetafileType--}
```
public boolean isMetafileType()
```


Bir görüntü formatının metafile türü olup olmadığını belirler.

**Returns:**
boolean - true ise bir görüntü biçimi metafile türündedir; aksi takdirde false.
### isUnknownType() {#isUnknownType--}
```
public boolean isUnknownType()
```


Bir görüntü formatının bilinmeyen tür olup olmadığını belirler.

**Returns:**
boolean - true ise bir görüntü biçimi bilinmeyen türdedir; aksi takdirde false.
### toString() {#toString--}
```
public String toString()
```


Bu ImageFormat nesnesini okunabilir bir dizeye dönüştürür.

**Returns:**
java.lang.String - Bu ImageFormat nesnesini temsil eden bir dize.
