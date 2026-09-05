---
title: "FontResolveEventArgs"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Menyediakan argumen untuk callback yang dipanggil ketika font diselesaikan."
type: docs
weight: 99
url: /id/java/com.aspose.tasks/fontresolveeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public final class FontResolveEventArgs extends System.EventArgs
```

Menyediakan argumen untuk callback yang dipanggil ketika font diselesaikan.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getRequestedFontName()](#getRequestedFontName--) | Mendapatkan nama font yang diminta. |
| [getResolvedFontName()](#getResolvedFontName--) | Mendapatkan nama font yang diresolusikan. |
| [setResolvedFontName(String value)](#setResolvedFontName-java.lang.String-) | Menetapkan nama font yang diresolusikan. |
### getRequestedFontName() {#getRequestedFontName--}
```
public final String getRequestedFontName()
```


Mendapatkan nama font yang diminta.

**Returns:**
java.lang.String - nama font yang diminta.
### getResolvedFontName() {#getResolvedFontName--}
```
public final String getResolvedFontName()
```


Mendapatkan nama font yang diresolusikan. Dapat diatur untuk mengontrol font yang digunakan untuk merender tampilan.

**Returns:**
java.lang.String - Nama font yang diminta jika font ditemukan atau nama font cadangan atau null jika font tidak dapat ditemukan.
### setResolvedFontName(String value) {#setResolvedFontName-java.lang.String-}
```
public final void setResolvedFontName(String value)
```


Menetapkan nama font yang diresolusikan. Dapat diatur untuk mengontrol font yang digunakan untuk merender tampilan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nama font yang diresolusikan. |

