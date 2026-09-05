---
title: "FontSettings"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Menentukan pengaturan font yang digunakan saat merender tampilan proyek."
type: docs
weight: 101
url: /id/java/com.aspose.tasks/fontsettings/
---

**Inheritance:**
java.lang.Object
```
public final class FontSettings
```

Menentukan pengaturan font yang digunakan saat merender tampilan proyek.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [FontSettings()](#FontSettings--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getDefaultFontName()](#getDefaultFontName--) | Mendapatkan font default (atau cadangan) untuk merender. |
| [getFontResolveCallback()](#getFontResolveCallback--) | Mendapatkan callback yang dapat digunakan untuk menyesuaikan font yang diresolusikan. |
| [getUseProjectDefaultFont()](#getUseProjectDefaultFont--) | Mendapatkan nilai yang menunjukkan apakah font default harus digunakan untuk merender. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Mengatur font default (atau cadangan) untuk merender. |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Mengatur folder tempat Aspose.Tasks mencari font TrueType saat merender tampilan proyek. |
| [setFontResolveCallback(FontResolveCallbackDelegate value)](#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-) | Mengatur callback yang dapat digunakan untuk menyesuaikan font yang diresolusikan. |
| [setUseProjectDefaultFont(boolean value)](#setUseProjectDefaultFont-boolean-) | Mengatur nilai yang menunjukkan apakah font default harus digunakan untuk merender. |
### FontSettings() {#FontSettings--}
```
public FontSettings()
```


### getDefaultFontName() {#getDefaultFontName--}
```
public final String getDefaultFontName()
```


Mendapatkan font default (atau cadangan) untuk merender.

**Returns:**
java.lang.String - font default (atau cadangan) untuk merender.
### getFontResolveCallback() {#getFontResolveCallback--}
```
public final FontResolveCallbackDelegate getFontResolveCallback()
```


Mendapatkan callback yang dapat digunakan untuk menyesuaikan font yang diresolusikan.

**Returns:**
[FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) - a callback which can be used to customize resolved fonts.
### getUseProjectDefaultFont() {#getUseProjectDefaultFont--}
```
public final boolean getUseProjectDefaultFont()
```


Mendapatkan nilai yang menunjukkan apakah font default harus digunakan untuk merender.

--------------------

Ketika nilai adalah False dan DefaultFontName ditentukan, mesin rendering akan menggunakan font yang ditentukan oleh DefaultFontName sebagai font cadangan. Jika tidak, font 'Arial' (jika terpasang) atau font 'Generic Sans Serif' akan digunakan sebagai font cadangan. Font cadangan digunakan selama rendering tampilan proyek ketika gaya teks merujuk pada font yang tidak terpasang pada sistem operasi saat ini. Untuk kontrol yang lebih besar atas resolusi font, Anda dapat menggunakan callback `FontResolveCallback`([getFontResolveCallback](../../com.aspose.tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose.tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-)).

**Returns:**
boolean - nilai yang menunjukkan apakah font default harus digunakan untuk rendering.
### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public final void setDefaultFontName(String value)
```


Mengatur font default (atau cadangan) untuk merender.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | font default (atau cadangan) untuk rendering. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public final void setFontFolders(String[] fontFolders, boolean recursive)
```


Mengatur folder tempat Aspose.Tasks mencari font TrueType saat merender tampilan proyek.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fontFolders | java.lang.String[] | Array folder yang berisi font TrueType. |
| recursive | boolean | Jika true, folder yang ditentukan akan dipindai secara rekursif. |

### setFontResolveCallback(FontResolveCallbackDelegate value) {#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-}
```
public final void setFontResolveCallback(FontResolveCallbackDelegate value)
```


Mengatur callback yang dapat digunakan untuk menyesuaikan font yang diresolusikan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) | callback yang dapat digunakan untuk menyesuaikan font yang diresolusikan. |

### setUseProjectDefaultFont(boolean value) {#setUseProjectDefaultFont-boolean-}
```
public final void setUseProjectDefaultFont(boolean value)
```


Mengatur nilai yang menunjukkan apakah font default harus digunakan untuk merender.

--------------------

Ketika nilai adalah False dan DefaultFontName ditentukan, mesin rendering akan menggunakan font yang ditentukan oleh DefaultFontName sebagai font cadangan. Jika tidak, font 'Arial' (jika terpasang) atau font 'Generic Sans Serif' akan digunakan sebagai font cadangan. Font cadangan digunakan selama rendering tampilan proyek ketika gaya teks merujuk pada font yang tidak terpasang pada sistem operasi saat ini. Untuk kontrol yang lebih besar atas resolusi font, Anda dapat menggunakan callback `FontResolveCallback`([getFontResolveCallback](../../com.aspose.tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose.tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-)).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah font default harus digunakan untuk rendering. |

