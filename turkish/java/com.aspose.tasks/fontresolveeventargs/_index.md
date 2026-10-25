---
title: "FontResolveEventArgs"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Yazı tipi çözüldüğünde çağrılan geri çağrı için argümanları sağlar."
type: docs
weight: 99
url: /tr/java/com.aspose.tasks/fontresolveeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public final class FontResolveEventArgs extends System.EventArgs
```

Yazı tipi çözüldüğünde çağrılan geri çağrı için argümanları sağlar.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getRequestedFontName()](#getRequestedFontName--) | İstenen yazı tipinin adını alır. |
| [getResolvedFontName()](#getResolvedFontName--) | Çözülmüş yazı tipinin adını alır. |
| [setResolvedFontName(String value)](#setResolvedFontName-java.lang.String-) | Çözülmüş yazı tipinin adını ayarlar. |
### getRequestedFontName() {#getRequestedFontName--}
```
public final String getRequestedFontName()
```


İstenen yazı tipinin adını alır.

**Returns:**
java.lang.String - istenen yazı tipinin adı.
### getResolvedFontName() {#getResolvedFontName--}
```
public final String getResolvedFontName()
```


Çözülmüş yazı tipinin adını alır. Görünümün render edilmesinde kullanılan yazı tiplerini kontrol etmek için ayarlanabilir.

**Returns:**
java.lang.String - Yazı tipi bulunursa istenen yazı tipinin adı, bulunamazsa yedek yazı tipinin adı veya bulunamazsa null.
### setResolvedFontName(String value) {#setResolvedFontName-java.lang.String-}
```
public final void setResolvedFontName(String value)
```


Çözülmüş yazı tipinin adını ayarlar. Görünümün render edilmesinde kullanılan yazı tiplerini kontrol etmek için ayarlanabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | çözülmüş yazı tipinin adı. |

