---
title: "PrinterSettings"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يحدد معلومات حول كيفية طباعة المستند بما في ذلك الطابعة التي تقوم بطباعته."
type: docs
weight: 215
url: /ar/java/com.aspose.tasks/printersettings/
---

**Inheritance:**
java.lang.Object
```
public class PrinterSettings
```

يحدد معلومات حول طريقة طباعة المستند، بما في ذلك الطابعة التي تقوم بطباعته.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [PrinterSettings()](#PrinterSettings--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getCollate()](#getCollate--) | يحصل على قيمة تشير إلى ما إذا كان المستند المطبوع مُجمّعًا. |
| [getCopies()](#getCopies--) | يحصل على عدد النسخ من المستند للطباعة. |
| [getFromPage()](#getFromPage--) | يحصل على رقم الصفحة الأولى للطباعة. |
| [getPrintFileName()](#getPrintFileName--) | يحصل على اسم الملف عند الطباعة إلى ملف. |
| [getPrinterName()](#getPrinterName--) | يحصل على اسم الطابعة المستخدمة. |
| [getSupportsColor()](#getSupportsColor--) | يحصل على قيمة تشير إلى ما إذا كانت هذه الطابعة تدعم الطباعة بالألوان. |
| [getToPage()](#getToPage--) | يحصل على رقم الصفحة الأخيرة للطباعة. |
| [isDefaultPrinter()](#isDefaultPrinter--) | يحصل على قيمة تشير إلى ما إذا كانت خاصية PrinterName تحدد الطابعة الافتراضية، باستثناء عندما يقوم المستخدم بتعيين PrinterName صراحةً. |
| [setCollate(boolean value)](#setCollate-boolean-) | يضبط قيمة تشير إلى ما إذا كان المستند المطبوع مُجمّعًا. |
| [setCopies(short value)](#setCopies-short-) | يضبط عدد النسخ من المستند للطباعة. |
| [setFromPage(int value)](#setFromPage-int-) | يضبط رقم الصفحة الأولى للطباعة. |
| [setPrintFileName(String value)](#setPrintFileName-java.lang.String-) | يضبط اسم الملف عند الطباعة إلى ملف. |
| [setPrinterName(String value)](#setPrinterName-java.lang.String-) | يضبط اسم الطابعة المستخدمة. |
| [setToPage(int value)](#setToPage-int-) | يضبط رقم الصفحة الأخيرة للطباعة. |
| [toString()](#toString--) | يوفر معلومات حول PrinterSettings في شكل سلسلة. |
### PrinterSettings() {#PrinterSettings--}
```
public PrinterSettings()
```


### getCollate() {#getCollate--}
```
public boolean getCollate()
```


يحصل على قيمة تشير إلى ما إذا كان المستند المطبوع مُجمّعًا.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان المستند المطبوع مُجمّعًا.
### getCopies() {#getCopies--}
```
public short getCopies()
```


يحصل على عدد النسخ من المستند للطباعة.

**Returns:**
short - عدد النسخ من المستند للطباعة.
### getFromPage() {#getFromPage--}
```
public int getFromPage()
```


يحصل على رقم الصفحة الأولى للطباعة.

**Returns:**
int - رقم الصفحة الأولى للطباعة.
### getPrintFileName() {#getPrintFileName--}
```
public String getPrintFileName()
```


يحصل على اسم الملف عند الطباعة إلى ملف.

**Returns:**
java.lang.String - اسم الملف، عند الطباعة إلى ملف.
### getPrinterName() {#getPrinterName--}
```
public String getPrinterName()
```


يحصل على اسم الطابعة المستخدمة.

**Returns:**
java.lang.String - اسم الطابعة التي سيتم استخدامها.
### getSupportsColor() {#getSupportsColor--}
```
public boolean getSupportsColor()
```


يحصل على قيمة تشير إلى ما إذا كانت هذه الطابعة تدعم الطباعة بالألوان.

**Returns:**
boolean - قيمة تشير إلى ما إذا كانت هذه الطابعة تدعم الطباعة بالألوان.
### getToPage() {#getToPage--}
```
public int getToPage()
```


يحصل على رقم الصفحة الأخيرة للطباعة.

**Returns:**
int - عدد الصفحة الأخيرة للطباعة.
### isDefaultPrinter() {#isDefaultPrinter--}
```
public boolean isDefaultPrinter()
```


يحصل على قيمة تشير إلى ما إذا كانت خاصية PrinterName تحدد الطابعة الافتراضية، باستثناء عندما يقوم المستخدم بتعيين PrinterName صراحةً.

**Returns:**
boolean - قيمة تشير إلى ما إذا كانت خاصية PrinterName تعين الطابعة الافتراضية.
### setCollate(boolean value) {#setCollate-boolean-}
```
public void setCollate(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان المستند المطبوع مُجمّعًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان المستند المطبوع مُرتّبًا. |

### setCopies(short value) {#setCopies-short-}
```
public void setCopies(short value)
```


يضبط عدد النسخ من المستند للطباعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | short | عدد النسخ من المستند للطباعة. |

### setFromPage(int value) {#setFromPage-int-}
```
public void setFromPage(int value)
```


يضبط رقم الصفحة الأولى للطباعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | رقم الصفحة الأولى للطباعة. |

### setPrintFileName(String value) {#setPrintFileName-java.lang.String-}
```
public void setPrintFileName(String value)
```


يضبط اسم الملف عند الطباعة إلى ملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | اسم الملف، عند الطباعة إلى ملف. |

### setPrinterName(String value) {#setPrinterName-java.lang.String-}
```
public void setPrinterName(String value)
```


يضبط اسم الطابعة المستخدمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | اسم الطابعة التي سيتم استخدامها. |

### setToPage(int value) {#setToPage-int-}
```
public void setToPage(int value)
```


يضبط رقم الصفحة الأخيرة للطباعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | عدد الصفحة الأخيرة للطباعة. |

### toString() {#toString--}
```
public String toString()
```


يوفر معلومات حول PrinterSettings في شكل سلسلة.

**Returns:**
java.lang.String - معلومات حول PrinterSettings بصيغة سلسلة.
