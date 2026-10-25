---
title: "PdfSaveOptions"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يسمح بتحديد خيارات إضافية عند تحويل صفحات المشروع إلى PDF."
type: docs
weight: 191
url: /ar/java/com.aspose.tasks/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class PdfSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

يسمح بتحديد خيارات إضافية عند تحويل صفحات المشروع إلى PDF.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | يُنشئ نسخة جديدة من الفئة [PdfSaveOptions](../../com.aspose/tasks/pdfsaveoptions) التي يمكن استخدامها لحفظ مستند بصيغة [SaveFileFormat](../../com.aspose/tasks/savefileformat). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getCompliance()](#getCompliance--) | يحصل على مستوى الامتثال المطلوب للمستند PDF المُنشأ. |
| [getEncryptionDetails()](#getEncryptionDetails--) | يحصل على تفاصيل التشفير. |
| [getFontSettings()](#getFontSettings--) | يحدد إعدادات الخط المستخدمة عند عرض رؤية المشروع. |
| [getPageSavingCallback()](#getPageSavingCallback--) | يحصل على رد نداء معرف من قبل المستخدم يُستخدم للحصول على تدفق إخراج لكل صفحة مُعالجة. |
| [getPages()](#getPages--) | يحصل على قائمة أرقام الصفحات التي سيتم حفظها عند حفظ تخطيط المشروع إلى ملفات منفصلة. |
| [getReduceFooterGap()](#getReduceFooterGap--) | يحصل على قيمة تشير إلى ما إذا كان يجب تقليل الفجوة بين المهمة الأخيرة وتذييل الصفحة. |
| [getSaveToSeparateFiles()](#getSaveToSeparateFiles--) | يحصل على قيمة تشير إلى ما إذا كان سيتم حفظ صفحات المشروع إلى ملفات منفصلة. |
| [getTextCompression()](#getTextCompression--) | يحصل على نوع الضغط الذي سيُستخدم لجميع تدفقات المحتوى باستثناء الصور. |
| [setCompliance(int value)](#setCompliance-int-) | يضبط مستوى الامتثال المطلوب للمستند PDF المُنشأ. |
| [setEncryptionDetails(PdfEncryptionDetails value)](#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-) | يضبط تفاصيل التشفير. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | يضبط رد نداء معرف من قبل المستخدم يُستخدم للحصول على تدفق إخراج لكل صفحة مُعالجة. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | يضبط قائمة أرقام الصفحات التي سيتم حفظها عند حفظ تخطيط المشروع إلى ملفات منفصلة. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب تقليل الفجوة بين المهمة الأخيرة وتذييل الصفحة. |
| [setSaveToSeparateFiles(boolean value)](#setSaveToSeparateFiles-boolean-) | يضبط قيمة تشير إلى ما إذا كان سيتم حفظ صفحات المشروع إلى ملفات منفصلة. |
| [setTextCompression(int value)](#setTextCompression-int-) | يضبط نوع الضغط الذي سيُستخدم لجميع تدفقات المحتوى باستثناء الصور. |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


يُنشئ نسخة جديدة من الفئة [PdfSaveOptions](../../com.aspose/tasks/pdfsaveoptions) التي يمكن استخدامها لحفظ مستند بصيغة [SaveFileFormat](../../com.aspose/tasks/savefileformat).

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public void copyOutputPropertiesFrom(SaveOptions source)
```


محجوز للاستخدام الداخلي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| source | [SaveOptions](../../com.aspose.tasks/saveoptions) | \{@inheritDoc\} |

### deepClone() {#deepClone--}
```
public SaveOptions deepClone()
```


محجوز للاستخدام الداخلي.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getCompliance() {#getCompliance--}
```
public final int getCompliance()
```


يحصل على مستوى الامتثال المطلوب للمستند PDF المُنشأ. الافتراضي هو [PdfCompliance.Pdf15](../../com.aspose/tasks/pdfcompliance\\#Pdf15).

**Returns:**
int - مستوى الامتثال المطلوب للمستند PDF المُنشأ.
### getEncryptionDetails() {#getEncryptionDetails--}
```
public final PdfEncryptionDetails getEncryptionDetails()
```


يحصل على تفاصيل التشفير. إذا لم يتم تعيينها، فلن يتم تنفيذ أي تشفير.

**Returns:**
[PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) - an encryption details.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


يحدد إعدادات الخط المستخدمة عند عرض رؤية المشروع.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


يحصل على رد نداء معرف من قبل المستخدم يُستخدم للحصول على تدفق إخراج لكل صفحة مُعالجة. يُطبق عندما يتم استخدام الخيار `SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose.tasks/pdfsaveoptions\\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose.tasks/pdfsaveoptions\\#setSaveToSeparateFiles-boolean-)).

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


يحصل على قائمة أرقام الصفحات التي سيتم حفظها عند حفظ تخطيط المشروع إلى ملفات منفصلة.

--------------------

سيتم حفظ جميع الصفحات إذا كانت هذه القائمة فارغة.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - قائمة أرقام الصفحات التي سيتم حفظها عند حفظ تخطيط المشروع إلى ملفات منفصلة.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


يحصل على قيمة تشير إلى ما إذا كان يجب تقليل الفجوة بين المهمة الأخيرة وتذييل الصفحة.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب تقليل الفجوة بين المهمة الأخيرة وتذييل الصفحة.
### getSaveToSeparateFiles() {#getSaveToSeparateFiles--}
```
public final boolean getSaveToSeparateFiles()
```


يحصل على قيمة تشير إلى ما إذا كان سيتم حفظ صفحات المشروع إلى ملفات منفصلة.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب حفظ صفحات المشروع في ملفات منفصلة.
### getTextCompression() {#getTextCompression--}
```
public final int getTextCompression()
```


يحصل على نوع الضغط الذي سيُستخدم لجميع تدفقات المحتوى باستثناء الصور. الافتراضي هو [PdfTextCompression.Flate](../../com.aspose.tasks/pdftextcompression\#Flate).

**Returns:**
int - نوع الضغط الذي سيُستخدم لجميع تدفقات المحتوى باستثناء الصور.
### setCompliance(int value) {#setCompliance-int-}
```
public final void setCompliance(int value)
```


يضبط مستوى الامتثال المطلوب للمستند PDF المُولد. الافتراضي هو [PdfCompliance.Pdf15](../../com.aspose.tasks/pdfcompliance\#Pdf15).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | مستوى الامتثال المطلوب للمستند PDF المُولد. |

### setEncryptionDetails(PdfEncryptionDetails value) {#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-}
```
public final void setEncryptionDetails(PdfEncryptionDetails value)
```


يضبط تفاصيل التشفير. إذا لم يتم ضبطها، فلن يتم تنفيذ أي تشفير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) | تفاصيل التشفير. |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


يضبط رد نداء معرف من قبل المستخدم يُستخدم للحصول على تدفق إخراج لكل صفحة مُعالجة. يُطبق عندما يتم استخدام خيار `SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose.tasks/pdfsaveoptions\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose.tasks/pdfsaveoptions\#setSaveToSeparateFiles-boolean-)).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | دالة رد نداء معرفة من قبل المستخدم تُستخدم للحصول على تدفق إخراج لكل صفحة مُصوَّرة. |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


يضبط قائمة أرقام الصفحات التي سيتم حفظها عند حفظ تخطيط المشروع إلى ملفات منفصلة.

--------------------

سيتم حفظ جميع الصفحات إذا كانت هذه القائمة فارغة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.List&lt;java.lang.Integer&gt; | قائمة أرقام الصفحات التي سيتم حفظها عند حفظ تخطيط المشروع في ملفات منفصلة. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب تقليل الفجوة بين المهمة الأخيرة وتذييل الصفحة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب تقليل الفجوة بين آخر مهمة وتذييل الصفحة. |

### setSaveToSeparateFiles(boolean value) {#setSaveToSeparateFiles-boolean-}
```
public final void setSaveToSeparateFiles(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان سيتم حفظ صفحات المشروع إلى ملفات منفصلة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب حفظ صفحات المشروع في ملفات منفصلة. |

### setTextCompression(int value) {#setTextCompression-int-}
```
public final void setTextCompression(int value)
```


يضبط نوع الضغط الذي سيُستخدم لجميع تدفقات المحتوى باستثناء الصور. الافتراضي هو [PdfTextCompression.Flate](../../com.aspose.tasks/pdftextcompression\#Flate).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | نوع الضغط الذي سيُستخدم لجميع تدفقات المحتوى باستثناء الصور. |

