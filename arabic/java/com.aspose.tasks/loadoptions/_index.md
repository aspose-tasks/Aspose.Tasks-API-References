---
title: "LoadOptions"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يسمح بتحديد معلمات تحميل إضافية عند تحميل مشروع من ملف أو تدفق."
type: docs
weight: 148
url: /ar/java/com.aspose.tasks/loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

يسمح بتحديد معلمات تحميل إضافية عند تحميل مشروع من ملف أو تدفق.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [LoadOptions()](#LoadOptions--) | ينشئ نسخة جديدة من الفئة [LoadOptions](../../com.aspose.tasks/loadoptions). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getCancellationToken()](#getCancellationToken--) | يحصل على رمز يمكن استخدامه لإلغاء عملية تحميل المشروع. |
| [getEncoding()](#getEncoding--) | يحصل على الترميز المستخدم لقراءة مشروع من صيغ HTML و MPX و XER و Primavera XML. |
| [getErrorHandler()](#getErrorHandler--) | يحصل على طريقة رد نداء لمعالجة أخطاء تحليل XML. |
| [getPassword()](#getPassword--) | يحصل على كلمة مرور الحماية. |
| [getPrimaveraReadOptions()](#getPrimaveraReadOptions--) | يحصل على نسخة محددة من الفئة [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) التي يمكن استخدامها لتخصيص سلوك تحميل صيغ Primavera (Primavera P6 XER أو Primavera P6 Xml). |
| [setCancellationToken(CancellationToken value)](#setCancellationToken-com.aspose.tasks.CancellationToken-) | يضبط رمزًا يمكن استخدامه لإلغاء عملية تحميل المشروع. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | يضبط الترميز المستخدم لقراءة مشروع من صيغ HTML و MPX و XER و Primavera XML. |
| [setErrorHandler(ParseErrorCallback value)](#setErrorHandler-com.aspose.tasks.ParseErrorCallback-) | يضبط طريقة رد نداء لمعالجة أخطاء تحليل XML. |
| [setPassword(String value)](#setPassword-java.lang.String-) | يضبط كلمة مرور الحماية. |
| [setPrimaveraReadOptions(PrimaveraReadOptions value)](#setPrimaveraReadOptions-com.aspose.tasks.PrimaveraReadOptions-) | يضبط نسخة محددة من الفئة [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) التي يمكن استخدامها لتخصيص سلوك تحميل صيغ Primavera (Primavera P6 XER أو Primavera P6 Xml). |
### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


ينشئ نسخة جديدة من الفئة [LoadOptions](../../com.aspose.tasks/loadoptions).

### getCancellationToken() {#getCancellationToken--}
```
public final CancellationToken getCancellationToken()
```


يحصل على رمز يمكن استخدامه لإلغاء عملية تحميل المشروع.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token which can be used to cancel a project loading operation.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


يحصل على الترميز المستخدم لقراءة مشروع من صيغ HTML و MPX و XER و Primavera XML. الترميز الافتراضي هو UTF8.

**Returns:**
java.nio.charset.Charset - الترميز المستخدم لقراءة مشروع من صيغ HTML و MPX و XER و Primavera XML.
### getErrorHandler() {#getErrorHandler--}
```
public final ParseErrorCallback getErrorHandler()
```


يحصل على طريقة رد نداء لمعالجة أخطاء تحليل XML.

**Returns:**
[ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) - a callback method to handle xml parse errors.
### getPassword() {#getPassword--}
```
public final String getPassword()
```


يحصل على كلمة مرور الحماية.

**Returns:**
java.lang.String - كلمة مرور الحماية.
### getPrimaveraReadOptions() {#getPrimaveraReadOptions--}
```
public final PrimaveraReadOptions getPrimaveraReadOptions()
```


يحصل على نسخة محددة من الفئة [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) التي يمكن استخدامها لتخصيص سلوك تحميل صيغ Primavera (Primavera P6 XER أو Primavera P6 Xml).

**Returns:**
[PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) - a specified instance of the [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) class which can be used to customize the behavior of loading Primavera formats (Primavera P6 XER or Primavera P6 Xml).
### setCancellationToken(CancellationToken value) {#setCancellationToken-com.aspose.tasks.CancellationToken-}
```
public final void setCancellationToken(CancellationToken value)
```


يضبط رمزًا يمكن استخدامه لإلغاء عملية تحميل المشروع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [CancellationToken](../../com.aspose.tasks/cancellationtoken) | رمز يمكن استخدامه لإلغاء عملية تحميل المشروع. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


يضبط الترميز المستخدم لقراءة مشروع من صيغ HTML و MPX و XER و Primavera XML. الترميز الافتراضي هو UTF8.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.nio.charset.Charset | الترميز المستخدم لقراءة مشروع من صيغ HTML و MPX و XER و Primavera XML. |

### setErrorHandler(ParseErrorCallback value) {#setErrorHandler-com.aspose.tasks.ParseErrorCallback-}
```
public final void setErrorHandler(ParseErrorCallback value)
```


يضبط طريقة رد نداء لمعالجة أخطاء تحليل XML.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | طريقة رد نداء لمعالجة أخطاء تحليل xml. |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


يضبط كلمة مرور الحماية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | كلمة مرور حماية. |

### setPrimaveraReadOptions(PrimaveraReadOptions value) {#setPrimaveraReadOptions-com.aspose.tasks.PrimaveraReadOptions-}
```
public final void setPrimaveraReadOptions(PrimaveraReadOptions value)
```


يضبط نسخة محددة من الفئة [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) التي يمكن استخدامها لتخصيص سلوك تحميل صيغ Primavera (Primavera P6 XER أو Primavera P6 Xml).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | مثال محدد من الفئة [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) التي يمكن استخدامها لتخصيص سلوك تحميل صيغ Primavera (Primavera P6 XER أو Primavera P6 Xml). |

