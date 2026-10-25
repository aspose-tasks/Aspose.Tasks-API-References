---
title: "FontResolveEventArgs"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يوفر الوسائط لرد النداء الذي يتم استدعاؤه عندما يتم حل الخط."
type: docs
weight: 99
url: /ar/java/com.aspose.tasks/fontresolveeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public final class FontResolveEventArgs extends System.EventArgs
```

يوفر الوسائط لرد النداء الذي يتم استدعاؤه عندما يتم حل الخط.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getRequestedFontName()](#getRequestedFontName--) | يحصل على اسم الخط المطلوب. |
| [getResolvedFontName()](#getResolvedFontName--) | يحصل على اسم الخط المحلول. |
| [setResolvedFontName(String value)](#setResolvedFontName-java.lang.String-) | يضبط اسم الخط المحلول. |
### getRequestedFontName() {#getRequestedFontName--}
```
public final String getRequestedFontName()
```


يحصل على اسم الخط المطلوب.

**Returns:**
java.lang.String - اسم الخط المطلوب.
### getResolvedFontName() {#getResolvedFontName--}
```
public final String getResolvedFontName()
```


يحصل على اسم الخط المحلول. يمكن ضبطه للتحكم في الخطوط المستخدمة لعرض المشهد.

**Returns:**
java.lang.String - اسم الخط المطلوب إذا تم العثور على الخط أو اسم الخط الاحتياطي أو null إذا لم يتم العثور على الخط.
### setResolvedFontName(String value) {#setResolvedFontName-java.lang.String-}
```
public final void setResolvedFontName(String value)
```


يضبط اسم الخط المحلول. يمكن ضبطه للتحكم في الخطوط المستخدمة لعرض المشهد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | اسم الخط المحلول. |

