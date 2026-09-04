---
title: "ResourceSavingArgs"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "تمثل هذه الفئة مجموعة من البيانات المتعلقة بحفظ ملفات الموارد الخارجية التي تحدث أثناء التحويل إلى تنسيق HTML."
type: docs
weight: 254
url: /ar/java/com.aspose.tasks/resourcesavingargs/
---

**Inheritance:**
java.lang.Object
```
public class ResourceSavingArgs
```

هذه الفئة تمثل مجموعة من البيانات المتعلقة بحفظ ملف المورد الخارجي الذي يحدث أثناء التحويل إلى تنسيق HTML.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [ResourceSavingArgs()](#ResourceSavingArgs--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [closeStreamIfRequired()](#closeStreamIfRequired--) | أغلق الدفق إذا كان KeepStreamOpen خاطئًا، وإلا قم بتفريغه. |
| [getFileName()](#getFileName--) | يحصل على اسم الملف المفترض الذي ينتقل من المحول إلى شفرة الطريقة المخصصة. |
| [getKeepStreamOpen()](#getKeepStreamOpen--) | يحصل على قيمة تشير إلى ما إذا كان الدفق سيبقى مفتوحًا بعد انتهاء حفظ الموارد. |
| [getStream()](#getStream--) | يحصل على المحتوى الثنائي للملف المحفوظ. |
| [getUri()](#getUri--) | يحصل على عنوان URI للموارد. |
| [setFileName(String value)](#setFileName-java.lang.String-) | يضبط اسم الملف المفترض الذي ينتقل من المحول إلى شفرة الطريقة المخصصة. |
| [setKeepStreamOpen(boolean value)](#setKeepStreamOpen-boolean-) | يضبط قيمة تشير إلى ما إذا كان الدفق سيبقى مفتوحًا بعد انتهاء حفظ الموارد. |
| [setStream(OutputStream value)](#setStream-java.io.OutputStream-) | يضبط المحتوى الثنائي للملف المحفوظ. |
| [setUri(String value)](#setUri-java.lang.String-) | يضبط عنوان URI للموارد. |
### ResourceSavingArgs() {#ResourceSavingArgs--}
```
public ResourceSavingArgs()
```


### closeStreamIfRequired() {#closeStreamIfRequired--}
```
public final void closeStreamIfRequired()
```


أغلق الدفق إذا كان KeepStreamOpen خاطئًا، وإلا قم بتفريغه.

### getFileName() {#getFileName--}
```
public final String getFileName()
```


يحصل على اسم الملف المفترض الذي ينتقل من المحول إلى شفرة الطريقة المخصصة. يمكن استخدامه في الشفرة المخصصة لتحديد كيفية معالجة الملف أو أين يتم حفظه.

**Returns:**
java.lang.String - اسم الملف المفترض الذي ينتقل من المحول إلى شفرة الطريقة المخصصة.
### getKeepStreamOpen() {#getKeepStreamOpen--}
```
public final boolean getKeepStreamOpen()
```


يحصل على قيمة تشير إلى ما إذا كان الدفق سيبقى مفتوحًا بعد انتهاء حفظ الموارد.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان الدفق سيبقى مفتوحًا بعد انتهاء حفظ الموارد.
### getStream() {#getStream--}
```
public final OutputStream getStream()
```


يحصل على المحتوى الثنائي للملف المحفوظ.

**Returns:**
java.io.OutputStream - المحتوى الثنائي للملف المحفوظ.
### getUri() {#getUri--}
```
public final String getUri()
```


يحصل على عنوان URI للموارد.

**Returns:**
java.lang.String - عنوان URI للموارد.
### setFileName(String value) {#setFileName-java.lang.String-}
```
public final void setFileName(String value)
```


يضبط اسم الملف المفترض الذي ينتقل من المحول إلى شفرة الطريقة المخصصة. يمكن استخدامه في الشفرة المخصصة لتحديد كيفية معالجة الملف أو أين يتم حفظه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | اسم الملف المفترض الذي ينتقل من المحول إلى شفرة الطريقة المخصصة. |

### setKeepStreamOpen(boolean value) {#setKeepStreamOpen-boolean-}
```
public final void setKeepStreamOpen(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان الدفق سيبقى مفتوحًا بعد انتهاء حفظ الموارد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان الدفق سيبقى مفتوحًا بعد انتهاء حفظ الموارد. |

### setStream(OutputStream value) {#setStream-java.io.OutputStream-}
```
public final void setStream(OutputStream value)
```


يضبط المحتوى الثنائي للملف المحفوظ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.io.OutputStream | المحتوى الثنائي للملف المحفوظ. |

### setUri(String value) {#setUri-java.lang.String-}
```
public final void setUri(String value)
```


يضبط عنوان URI للموارد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | معرف URI للمورد. |

