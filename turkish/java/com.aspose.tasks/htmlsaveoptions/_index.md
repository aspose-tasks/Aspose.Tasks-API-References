---
title: "HtmlSaveOptions"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Proje sayfalarını HTML'ye işlerken ek seçenekler belirtmeye izin verir."
type: docs
weight: 132
url: /tr/java/com.aspose.tasks/htmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class HtmlSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Proje sayfalarını HTML'ye işlerken ek seçenekler belirtmeye izin verir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [HtmlSaveOptions()](#HtmlSaveOptions--) | Yeni bir [HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getCssSavingCallback()](#getCssSavingCallback--) | CSS'i depolamak için kaynak oluşturacak callback'i alır. |
| [getCssStylePrefix()](#getCssStylePrefix--) | CSS stil önekini alır. |
| [getExportCss()](#getExportCss--) | CSS'in dışa aktarım şeklini alır. |
| [getExportFonts()](#getExportFonts--) | Yazı tiplerinin dışa aktarım şeklini alır. |
| [getExportImages()](#getExportImages--) | Görüntülerin dışa aktarım şeklini alır. |
| [getFontFaceTypes()](#getFontFaceTypes--) | Yazı tipi yüz türlerini alır. |
| [getFontSavingCallback()](#getFontSavingCallback--) | Yazı tipini depolamak için kaynak oluşturacak callback'i alır. |
| [getFontSettings()](#getFontSettings--) | Proje görünümü oluşturulurken kullanılan yazı tipi ayarlarını belirtir. |
| [getImageSavingCallback()](#getImageSavingCallback--) | Yazı tipini depolamak için kaynak oluşturacak callback'i alır. |
| [getIncludeProjectNameInPageHeader()](#getIncludeProjectNameInPageHeader--) | Proje adının HTML sayfa başlığında dahil edilip edilmeyeceğini gösteren değeri alır. |
| [getIncludeProjectNameInTitle()](#getIncludeProjectNameInTitle--) | Proje adının HTML başlığında dahil edilip edilmeyeceğini gösteren değeri alır. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Her işlenen sayfa için çıktı akışı elde etmekte kullanılan kullanıcı tanımlı callback'i alır. |
| [getPages()](#getPages--) | Proje düzeni işlenirken kaydedilecek sayfa numaralarının listesini alır. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Son görev ile alt bilgi arasındaki boşluğun azaltılıp azaltılmayacağını gösteren değeri alır. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Proje düzeni işlenirken degrade fırçası kullanılıp kullanılmayacağını gösteren değeri alır. |
| [setCssSavingCallback(ICssSavingCallback value)](#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-) | CSS'i depolamak için kaynak oluşturacak callback'i ayarlar. |
| [setCssStylePrefix(String value)](#setCssStylePrefix-java.lang.String-) | CSS stil önekini ayarlar. |
| [setExportCss(int value)](#setExportCss-int-) | CSS'in dışa aktarım şeklini ayarlar. |
| [setExportFonts(int value)](#setExportFonts-int-) | Yazı tiplerinin dışa aktarım şeklini ayarlar. |
| [setExportImages(int value)](#setExportImages-int-) | Görüntülerin dışa aktarım şeklini ayarlar. |
| [setFontFaceTypes(int value)](#setFontFaceTypes-int-) | Yazı tipi yüzü türlerini ayarlar. |
| [setFontSavingCallback(IFontSavingCallback value)](#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-) | Yazı tipini depolamak için kaynak oluşturacak geri aramayı ayarlar. |
| [setImageSavingCallback(IImageSavingCallback value)](#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-) | Yazı tipini depolamak için kaynak oluşturacak geri aramayı ayarlar. |
| [setIncludeProjectNameInPageHeader(boolean value)](#setIncludeProjectNameInPageHeader-boolean-) | Proje adının HTML sayfa başlığında dahil edilip edilmeyeceğini gösteren bir değeri ayarlar. |
| [setIncludeProjectNameInTitle(boolean value)](#setIncludeProjectNameInTitle-boolean-) | Proje adının HTML başlığında dahil edilip edilmeyeceğini gösteren bir değeri ayarlar. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Her render edilen sayfa için bir çıktı akışı almakta kullanılan kullanıcı tanımlı geri aramayı ayarlar. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Proje düzeni render edilirken kaydedilecek sayfa numaralarının bir listesini ayarlar. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Son görev ile alt bilgi arasındaki boşluğun azaltılıp azaltılmayacağını gösteren bir değeri ayarlar. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Proje düzeni render edilirken degrade fırçasının kullanılıp kullanılmayacağını gösteren bir değeri ayarlar. |
### HtmlSaveOptions() {#HtmlSaveOptions--}
```
public HtmlSaveOptions()
```


Yeni bir [HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions) sınıfı örneği başlatır.

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
### getCssSavingCallback() {#getCssSavingCallback--}
```
public final ICssSavingCallback getCssSavingCallback()
```


CSS'i depolamak için kaynak oluşturacak callback'i alır.

**Returns:**
[ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) - the callback that is called to create resource to store CSS.
### getCssStylePrefix() {#getCssStylePrefix--}
```
public final String getCssStylePrefix()
```


CSS stil önekini alır.

**Returns:**
java.lang.String - CSS stil öneki.
### getExportCss() {#getExportCss--}
```
public final int getExportCss()
```


CSS'in dışa aktarım şeklini alır.

**Returns:**
int - CSS'nin dışa aktarım şekli.
### getExportFonts() {#getExportFonts--}
```
public final int getExportFonts()
```


Yazı tiplerinin dışa aktarım şeklini alır.

**Returns:**
int - yazı tiplerinin dışa aktarım şekli.
### getExportImages() {#getExportImages--}
```
public final int getExportImages()
```


Görüntülerin dışa aktarım şeklini alır.

**Returns:**
int - görüntülerin dışa aktarım şekli.
### getFontFaceTypes() {#getFontFaceTypes--}
```
public final int getFontFaceTypes()
```


Yazı tipi yüz türlerini alır.

Değer: Yazı tipi yüzü türleri.

**Returns:**
int - yazı tipi yüzü türleri.
### getFontSavingCallback() {#getFontSavingCallback--}
```
public final IFontSavingCallback getFontSavingCallback()
```


Yazı tipini depolamak için kaynak oluşturacak callback'i alır.

**Returns:**
[IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) - the callback that is called to create resource to store font.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Proje görünümü oluşturulurken kullanılan yazı tipi ayarlarını belirtir.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getImageSavingCallback() {#getImageSavingCallback--}
```
public final IImageSavingCallback getImageSavingCallback()
```


Yazı tipini depolamak için kaynak oluşturacak callback'i alır.

**Returns:**
[IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) - the callback that is called to create resource to store font.
### getIncludeProjectNameInPageHeader() {#getIncludeProjectNameInPageHeader--}
```
public final boolean getIncludeProjectNameInPageHeader()
```


Proje adının HTML sayfa başlığında dahil edilip edilmeyeceğini gösteren değeri alır.

**Returns:**
boolean - proje adının HTML sayfa başlığında dahil edilip edilmeyeceğini gösteren bir değer.
### getIncludeProjectNameInTitle() {#getIncludeProjectNameInTitle--}
```
public final boolean getIncludeProjectNameInTitle()
```


Proje adının HTML başlığında dahil edilip edilmeyeceğini gösteren değeri alır.

**Returns:**
boolean - proje adının HTML başlığında dahil edilip edilmeyeceğini gösteren bir değer.
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


Proje düzeni işlenirken kaydedilecek sayfa numaralarının listesini alır.

--------------------

Bu liste boş ise tüm proje sayfaları kaydedilecektir.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - Proje düzeni render edilirken kaydedilecek sayfa numaralarının bir listesi.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Son görev ile alt bilgi arasındaki boşluğun azaltılıp azaltılmayacağını gösteren değeri alır.

**Returns:**
boolean - son görev ile alt bilgi arasındaki boşluğun azaltılıp azaltılmayacağını gösteren bir değer.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Proje düzeni işlenirken degrade fırçası kullanılıp kullanılmayacağını gösteren değeri alır.

--------------------

HTML'ye render edilirken degrade fırçasının kullanımı şu anda desteklenmemektedir.

**Returns:**
boolean - proje düzeni render edilirken degrade fırçasının kullanılıp kullanılmayacağını gösteren bir değer.
### setCssSavingCallback(ICssSavingCallback value) {#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-}
```
public final void setCssSavingCallback(ICssSavingCallback value)
```


CSS'i depolamak için kaynak oluşturacak callback'i ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) | CSS'yi depolamak için kaynak oluşturacak geri aramayı. |

### setCssStylePrefix(String value) {#setCssStylePrefix-java.lang.String-}
```
public final void setCssStylePrefix(String value)
```


CSS stil önekini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | CSS stil öneki. |

### setExportCss(int value) {#setExportCss-int-}
```
public final void setExportCss(int value)
```


CSS'in dışa aktarım şeklini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | CSS'nin dışa aktarılma şekli. |

### setExportFonts(int value) {#setExportFonts-int-}
```
public final void setExportFonts(int value)
```


Yazı tiplerinin dışa aktarım şeklini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | Yazı tiplerinin dışa aktarılma şekli. |

### setExportImages(int value) {#setExportImages-int-}
```
public final void setExportImages(int value)
```


Görüntülerin dışa aktarım şeklini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | Görüntülerin dışa aktarılma şekli. |

### setFontFaceTypes(int value) {#setFontFaceTypes-int-}
```
public final void setFontFaceTypes(int value)
```


Yazı tipi yüzü türlerini ayarlar.

Değer: Yazı tipi yüzü türleri.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | Yazı tipi yüzü türleri. |

### setFontSavingCallback(IFontSavingCallback value) {#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-}
```
public final void setFontSavingCallback(IFontSavingCallback value)
```


Yazı tipini depolamak için kaynak oluşturacak geri aramayı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) | Yazı tipini depolamak için kaynak oluşturacak callback. |

### setImageSavingCallback(IImageSavingCallback value) {#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-}
```
public final void setImageSavingCallback(IImageSavingCallback value)
```


Yazı tipini depolamak için kaynak oluşturacak geri aramayı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) | Yazı tipini depolamak için kaynak oluşturacak callback. |

### setIncludeProjectNameInPageHeader(boolean value) {#setIncludeProjectNameInPageHeader-boolean-}
```
public final void setIncludeProjectNameInPageHeader(boolean value)
```


Proje adının HTML sayfa başlığında dahil edilip edilmeyeceğini gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | HTML sayfa başlığında proje adının dahil edilip edilmeyeceğini gösteren bir değer. |

### setIncludeProjectNameInTitle(boolean value) {#setIncludeProjectNameInTitle-boolean-}
```
public final void setIncludeProjectNameInTitle(boolean value)
```


Proje adının HTML başlığında dahil edilip edilmeyeceğini gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | HTML başlığında proje adının dahil edililip edilmeyeceğini gösteren bir değer. |

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


Proje düzeni render edilirken kaydedilecek sayfa numaralarının bir listesini ayarlar.

--------------------

Bu liste boş ise tüm proje sayfaları kaydedilecektir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.List&lt;java.lang.Integer&gt; | Proje düzeni işlenirken kaydedilecek sayfa numaralarının listesi. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Son görev ile alt bilgi arasındaki boşluğun azaltılıp azaltılmayacağını gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | Son görev ile altbilgi arasındaki boşluğun azaltılıp azaltılmayacağını gösteren bir değer. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Proje düzeni render edilirken degrade fırçasının kullanılıp kullanılmayacağını gösteren bir değeri ayarlar.

--------------------

HTML'ye render edilirken degrade fırçasının kullanımı şu anda desteklenmemektedir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | Proje düzeni işlenirken degrade fırça kullanılıp kullanılmayacağını gösteren bir değer. |

