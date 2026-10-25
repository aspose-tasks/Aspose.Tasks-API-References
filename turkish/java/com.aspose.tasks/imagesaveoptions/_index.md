---
title: "ImageSaveOptions"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Proje sayfalarını görüntülere işlerken ek seçenekler belirtmeye izin verir."
type: docs
weight: 134
url: /tr/java/com.aspose.tasks/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class ImageSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Proje sayfalarını görüntülere işlerken ek seçenekler belirtmeye izin verir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ImageSaveOptions(int saveFormat)](#ImageSaveOptions-int-) | Yeni bir [ImageSaveOptions](../../com.aspose.tasks/imagesaveoptions) sınıfının örneğini başlatır; bu sınıf, oluşturulan görüntüleri TIFF, PNG, BMP veya JPEG formatlarında kaydetmek için kullanılabilir. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getFontSettings()](#getFontSettings--) | Proje görünümü oluşturulurken kullanılan yazı tipi ayarlarını belirtir. |
| [getHorizontalResolution()](#getHorizontalResolution--) | Yatay çözünürlüğü dpi cinsinden alır. |
| [getJpegQuality()](#getJpegQuality--) | JPEG kalitesini alır. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Her işlenen sayfa için çıktı akışı elde etmekte kullanılan kullanıcı tanımlı callback'i alır. |
| [getPages()](#getPages--) | Proje düzeni ayrı dosyalara kaydedilirken kaydedilecek sayfa numaralarının bir listesini alır. |
| [getPixelFormat()](#getPixelFormat--) | Görüntüdeki her piksel için renk verisinin formatını alır. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Son görev ile alt bilgi arasındaki boşluğun azaltılıp azaltılmayacağını gösteren değeri alır. |
| [getTiffCompression()](#getTiffCompression--) | Oluşturulan görüntüler TIFF formatında kaydedilirken uygulanacak sıkıştırma türünü alır. |
| [getVerticalResolution()](#getVerticalResolution--) | Dikey çözünürlüğü dpi cinsinden alır. |
| [setHorizontalResolution(float value)](#setHorizontalResolution-float-) | Yatay çözünürlüğü dpi cinsinden ayarlar. |
| [setJpegQuality(int value)](#setJpegQuality-int-) | JPEG kalitesini ayarlar. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Her render edilen sayfa için bir çıktı akışı almakta kullanılan kullanıcı tanımlı geri aramayı ayarlar. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Proje düzeni ayrı dosyalara kaydedilirken kaydedilecek sayfa numaralarının bir listesini ayarlar. |
| [setPixelFormat(int value)](#setPixelFormat-int-) | Görüntüdeki her piksel için renk verisinin formatını ayarlar. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Son görev ile alt bilgi arasındaki boşluğun azaltılıp azaltılmayacağını gösteren bir değeri ayarlar. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Oluşturulan görüntüler TIFF formatında kaydedilirken uygulanacak sıkıştırma türünü ayarlar. |
| [setVerticalResolution(float value)](#setVerticalResolution-float-) | Dikey çözünürlüğü dpi cinsinden ayarlar. |
### ImageSaveOptions(int saveFormat) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int saveFormat)
```


Yeni bir [ImageSaveOptions](../../com.aspose.tasks/imagesaveoptions) sınıfının örneğini başlatır; bu sınıf, oluşturulan görüntüleri TIFF, PNG, BMP veya JPEG formatlarında kaydetmek için kullanılabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| saveFormat | int | TIFF, PNG, BMP veya JPEG[SaveFileFormat](../../com.aspose.tasks/savefileformat) olabilir. |

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public final void copyOutputPropertiesFrom(SaveOptions source)
```


Dahili kullanım için ayrılmıştır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | [SaveOptions](../../com.aspose.tasks/saveoptions) | \{@inheritDoc\} |

### deepClone() {#deepClone--}
```
public SaveOptions deepClone()
```


Dahili kullanım için ayrılmıştır.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Proje görünümü oluşturulurken kullanılan yazı tipi ayarlarını belirtir.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getHorizontalResolution() {#getHorizontalResolution--}
```
public final float getHorizontalResolution()
```


Yatay çözünürlüğü dpi cinsinden alır.

**Returns:**
float - yatay çözünürlük dpi cinsinden.
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


JPEG kalitesini alır. İzin verilen değer aralığı 0..100'dür.

**Returns:**
int - JPEG kalitesi.
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Her işlenen sayfa için çıktı akışı elde etmekte kullanılan kullanıcı tanımlı callback'i alır.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


Proje düzeni ayrı dosyalara kaydedilirken kaydedilecek sayfa numaralarının bir listesini alır.

--------------------

Bu liste boşsa tüm sayfalar kaydedilir.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - proje düzeni ayrı dosyalara kaydedilirken kaydedilecek sayfa numaralarının bir listesi.
### getPixelFormat() {#getPixelFormat--}
```
public final int getPixelFormat()
```


Görüntüdeki her piksel için renk verisinin formatını alır.

**Returns:**
int - görüntüdeki her piksel için renk verisinin formatı.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Son görev ile alt bilgi arasındaki boşluğun azaltılıp azaltılmayacağını gösteren değeri alır.

**Returns:**
boolean - son görev ile alt bilgi arasındaki boşluğun azaltılıp azaltılmayacağını gösteren bir değer.
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


Oluşturulan görüntüler TIFF formatında kaydedilirken uygulanacak sıkıştırma türünü alır.

--------------------

Yalnızca TIFF olarak kaydederken etkili olur. Varsayılan değer `TiffCompressionLZW`([getTiffCompression()](../../com.aspose.tasks/imagesaveoptions\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\#setTiffCompression-int-)).

**Returns:**
int - oluşturulan görüntüler TIFF formatında kaydedilirken uygulanacak sıkıştırma türü.
### getVerticalResolution() {#getVerticalResolution--}
```
public final float getVerticalResolution()
```


Dikey çözünürlüğü dpi cinsinden alır.

**Returns:**
float - dikey çözünürlük dpi cinsinden.
### setHorizontalResolution(float value) {#setHorizontalResolution-float-}
```
public final void setHorizontalResolution(float value)
```


Yatay çözünürlüğü dpi cinsinden ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | float | yatay çözünürlük dpi cinsinden. |

### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


JPEG kalitesini ayarlar. İzin verilen değer aralığı 0..100'dür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | bir JPEG kalitesi. |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Her render edilen sayfa için bir çıktı akışı almakta kullanılan kullanıcı tanımlı geri aramayı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | Her işlenen sayfa için bir çıktı akışı almakta kullanılan kullanıcı tanımlı callback. |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


Proje düzeni ayrı dosyalara kaydedilirken kaydedilecek sayfa numaralarının bir listesini ayarlar.

--------------------

Bu liste boşsa tüm sayfalar kaydedilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.List&lt;java.lang.Integer&gt; | proje düzeni ayrı dosyalara kaydedilirken kaydedilecek sayfa numaralarının listesi. |

### setPixelFormat(int value) {#setPixelFormat-int-}
```
public final void setPixelFormat(int value)
```


Görüntüdeki her piksel için renk verisinin formatını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | görüntüdeki her piksel için renk verisinin biçimi. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Son görev ile alt bilgi arasındaki boşluğun azaltılıp azaltılmayacağını gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | Son görev ile altbilgi arasındaki boşluğun azaltılıp azaltılmayacağını gösteren bir değer. |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


Oluşturulan görüntüler TIFF formatında kaydedilirken uygulanacak sıkıştırma türünü ayarlar.

--------------------

Yalnızca TIFF olarak kaydederken etkili olur. Varsayılan değer `TiffCompressionLZW`([getTiffCompression()](../../com.aspose.tasks/imagesaveoptions\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\#setTiffCompression-int-)).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | oluşturulan görüntüler TIFF formatına kaydedilirken uygulanacak sıkıştırma türü. |

### setVerticalResolution(float value) {#setVerticalResolution-float-}
```
public final void setVerticalResolution(float value)
```


Dikey çözünürlüğü dpi cinsinden ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | float | dikey çözünürlük dpi cinsinden. |

