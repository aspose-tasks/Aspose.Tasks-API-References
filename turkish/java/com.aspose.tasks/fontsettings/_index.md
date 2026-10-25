---
title: "FontSettings"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Projeler görünümü işlenirken kullanılan yazı tipi ayarlarını belirtir."
type: docs
weight: 101
url: /tr/java/com.aspose.tasks/fontsettings/
---

**Inheritance:**
java.lang.Object
```
public final class FontSettings
```

Proje görünümü oluşturulurken kullanılan yazı tipi ayarlarını belirtir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [FontSettings()](#FontSettings--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getDefaultFontName()](#getDefaultFontName--) | İşleme için varsayılan (veya yedek) yazı tipini alır. |
| [getFontResolveCallback()](#getFontResolveCallback--) | Çözülmüş yazı tiplerini özelleştirmek için kullanılabilecek bir geri çağırma alır. |
| [getUseProjectDefaultFont()](#getUseProjectDefaultFont--) | İşleme için varsayılan yazı tipinin kullanılmasını gerekip gerektirmediğini belirten bir değeri alır. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | İşleme için varsayılan (veya yedek) yazı tipini ayarlar. |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Projeler görünümü işlenirken Aspose.Tasks'in TrueType yazı tiplerini aradığı klasörleri ayarlar. |
| [setFontResolveCallback(FontResolveCallbackDelegate value)](#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-) | Çözülmüş yazı tiplerini özelleştirmek için kullanılabilecek bir geri çağırma ayarlar. |
| [setUseProjectDefaultFont(boolean value)](#setUseProjectDefaultFont-boolean-) | İşleme için varsayılan yazı tipinin kullanılmasını gerekip gerektirmediğini belirten bir değeri ayarlar. |
### FontSettings() {#FontSettings--}
```
public FontSettings()
```


### getDefaultFontName() {#getDefaultFontName--}
```
public final String getDefaultFontName()
```


İşleme için varsayılan (veya yedek) yazı tipini alır.

**Returns:**
java.lang.String - işleme için varsayılan (veya yedek) yazı tipi.
### getFontResolveCallback() {#getFontResolveCallback--}
```
public final FontResolveCallbackDelegate getFontResolveCallback()
```


Çözülmüş yazı tiplerini özelleştirmek için kullanılabilecek bir geri çağırma alır.

**Returns:**
[FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) - a callback which can be used to customize resolved fonts.
### getUseProjectDefaultFont() {#getUseProjectDefaultFont--}
```
public final boolean getUseProjectDefaultFont()
```


İşleme için varsayılan yazı tipinin kullanılmasını gerekip gerektirmediğini belirten bir değeri alır.

--------------------

Değer False olduğunda ve DefaultFontName belirtildiğinde, render motoru DefaultFontName tarafından belirtilen yazı tipini yedek yazı tipi olarak kullanır. Aksi takdirde 'Arial' (yüklüyse) veya 'Generic Sans Serif' yazı tipleri yedek yazı tipi olarak kullanılır. Yedek yazı tipi, bir metin stilinin mevcut işletim sisteminde yüklü olmayan bir yazı tipine başvurduğu proje görünümü render edilirken kullanılır. Yazı tipi çözümlemesi üzerinde daha fazla kontrol için `FontResolveCallback`([getFontResolveCallback](../../com.aspose.tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose.tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-)) geri çağrısını kullanabilirsiniz.

**Returns:**
boolean - render için varsayılan yazı tipinin kullanılmasını gösteren bir değer.
### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public final void setDefaultFontName(String value)
```


İşleme için varsayılan (veya yedek) yazı tipini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | render için varsayılan (veya yedek) yazı tipi. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public final void setFontFolders(String[] fontFolders, boolean recursive)
```


Projeler görünümü işlenirken Aspose.Tasks'in TrueType yazı tiplerini aradığı klasörleri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fontFolders | java.lang.String[] | TrueType yazı tiplerini içeren klasörlerin bir dizisi. |
| recursive | boolean | Doğru ise belirtilen klasörler özyinelemeli olarak taranacaktır. |

### setFontResolveCallback(FontResolveCallbackDelegate value) {#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-}
```
public final void setFontResolveCallback(FontResolveCallbackDelegate value)
```


Çözülmüş yazı tiplerini özelleştirmek için kullanılabilecek bir geri çağırma ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) | çözülmüş yazı tiplerini özelleştirmek için kullanılabilecek bir geri çağrı. |

### setUseProjectDefaultFont(boolean value) {#setUseProjectDefaultFont-boolean-}
```
public final void setUseProjectDefaultFont(boolean value)
```


İşleme için varsayılan yazı tipinin kullanılmasını gerekip gerektirmediğini belirten bir değeri ayarlar.

--------------------

Değer False olduğunda ve DefaultFontName belirtildiğinde, render motoru DefaultFontName tarafından belirtilen yazı tipini yedek yazı tipi olarak kullanır. Aksi takdirde 'Arial' (yüklüyse) veya 'Generic Sans Serif' yazı tipleri yedek yazı tipi olarak kullanılır. Yedek yazı tipi, bir metin stilinin mevcut işletim sisteminde yüklü olmayan bir yazı tipine başvurduğu proje görünümü render edilirken kullanılır. Yazı tipi çözümlemesi üzerinde daha fazla kontrol için `FontResolveCallback`([getFontResolveCallback](../../com.aspose.tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose.tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-)) geri çağrısını kullanabilirsiniz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | render için varsayılan yazı tipinin kullanılmasını gösteren bir değer. |

