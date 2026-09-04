---
title: "ImageSaveOptions"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يسمح بتحديد خيارات إضافية عند تحويل صفحات المشروع إلى صور."
type: docs
weight: 134
url: /ar/java/com.aspose.tasks/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class ImageSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

يسمح بتحديد خيارات إضافية عند تحويل صفحات المشروع إلى صور.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [ImageSaveOptions(int saveFormat)](#ImageSaveOptions-int-) | يُنشئ مثلاً جديداً من الفئة [ImageSaveOptions](../../com.aspose.tasks/imagesaveoptions) التي يمكن استخدامها لحفظ الصور المُصدَّرة بتنسيقات TIFF أو PNG أو BMP أو JPEG. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getFontSettings()](#getFontSettings--) | يحدد إعدادات الخط المستخدمة عند عرض رؤية المشروع. |
| [getHorizontalResolution()](#getHorizontalResolution--) | يحصل على الدقة الأفقية بوحدة dpi. |
| [getJpegQuality()](#getJpegQuality--) | يحصل على جودة JPEG. |
| [getPageSavingCallback()](#getPageSavingCallback--) | يحصل على رد نداء معرف من قبل المستخدم يُستخدم للحصول على تدفق إخراج لكل صفحة مُعالجة. |
| [getPages()](#getPages--) | يحصل على قائمة بأرقام الصفحات لحفظها عند حفظ تخطيط المشروع إلى ملفات منفصلة. |
| [getPixelFormat()](#getPixelFormat--) | يحصل على تنسيق بيانات اللون لكل بكسل في الصورة. |
| [getReduceFooterGap()](#getReduceFooterGap--) | يحصل على قيمة تشير إلى ما إذا كان يجب تقليل الفجوة بين المهمة الأخيرة وتذييل الصفحة. |
| [getTiffCompression()](#getTiffCompression--) | يحصل على نوع الضغط الذي يُطبق عند حفظ الصور المولدة بتنسيق TIFF. |
| [getVerticalResolution()](#getVerticalResolution--) | يحصل على الدقة العمودية بوحدة dpi. |
| [setHorizontalResolution(float value)](#setHorizontalResolution-float-) | يضبط الدقة الأفقية بوحدة dpi. |
| [setJpegQuality(int value)](#setJpegQuality-int-) | يضبط جودة JPEG. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | يضبط رد نداء معرف من قبل المستخدم يُستخدم للحصول على تدفق إخراج لكل صفحة مُعالجة. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | يضبط قائمة بأرقام الصفحات لحفظها عند حفظ تخطيط المشروع إلى ملفات منفصلة. |
| [setPixelFormat(int value)](#setPixelFormat-int-) | يضبط تنسيق بيانات اللون لكل بكسل في الصورة. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب تقليل الفجوة بين المهمة الأخيرة وتذييل الصفحة. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | يضبط نوع الضغط الذي يُطبق عند حفظ الصور المولدة بتنسيق TIFF. |
| [setVerticalResolution(float value)](#setVerticalResolution-float-) | يضبط الدقة العمودية بوحدة dpi. |
### ImageSaveOptions(int saveFormat) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int saveFormat)
```


يُنشئ مثلاً جديداً من الفئة [ImageSaveOptions](../../com.aspose.tasks/imagesaveoptions) التي يمكن استخدامها لحفظ الصور المُصدَّرة بتنسيقات TIFF أو PNG أو BMP أو JPEG.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| saveFormat | int | يمكن أن يكون TIFF أو PNG أو BMP أو JPEG[SaveFileFormat](../../com.aspose.tasks/savefileformat). |

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public final void copyOutputPropertiesFrom(SaveOptions source)
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
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


يحدد إعدادات الخط المستخدمة عند عرض رؤية المشروع.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getHorizontalResolution() {#getHorizontalResolution--}
```
public final float getHorizontalResolution()
```


يحصل على الدقة الأفقية بوحدة dpi.

**Returns:**
float - الدقة الأفقية بوحدة dpi.
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


يحصل على جودة JPEG. النطاق المسموح للقيمة هو 0..100.

**Returns:**
int - جودة JPEG.
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


يحصل على رد نداء معرف من قبل المستخدم يُستخدم للحصول على تدفق إخراج لكل صفحة مُعالجة.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


يحصل على قائمة بأرقام الصفحات لحفظها عند حفظ تخطيط المشروع إلى ملفات منفصلة.

--------------------

سيتم حفظ جميع الصفحات إذا كانت هذه القائمة فارغة.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - قائمة بأرقام الصفحات لحفظها عند حفظ تخطيط المشروع إلى ملفات منفصلة.
### getPixelFormat() {#getPixelFormat--}
```
public final int getPixelFormat()
```


يحصل على تنسيق بيانات اللون لكل بكسل في الصورة.

**Returns:**
int - تنسيق بيانات اللون لكل بكسل في الصورة.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


يحصل على قيمة تشير إلى ما إذا كان يجب تقليل الفجوة بين المهمة الأخيرة وتذييل الصفحة.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب تقليل الفجوة بين المهمة الأخيرة وتذييل الصفحة.
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


يحصل على نوع الضغط الذي يُطبق عند حفظ الصور المولدة بتنسيق TIFF.

--------------------

يؤثر فقط عند الحفظ إلى TIFF. القيمة الافتراضية هي `TiffCompressionLZW`([getTiffCompression()](../../com.aspose.tasks/imagesaveoptions\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\#setTiffCompression-int-)).

**Returns:**
int - نوع الضغط الذي يُطبق عند حفظ الصور المولدة بتنسيق TIFF.
### getVerticalResolution() {#getVerticalResolution--}
```
public final float getVerticalResolution()
```


يحصل على الدقة العمودية بوحدة dpi.

**Returns:**
float - الدقة العمودية بوحدة dpi.
### setHorizontalResolution(float value) {#setHorizontalResolution-float-}
```
public final void setHorizontalResolution(float value)
```


يضبط الدقة الأفقية بوحدة dpi.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float | دقة الأفقية بوحدة dpi. |

### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


يضبط جودة JPEG. النطاق المسموح للقيمة هو 0..100.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | جودة JPEG. |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


يضبط رد نداء معرف من قبل المستخدم يُستخدم للحصول على تدفق إخراج لكل صفحة مُعالجة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | دالة رد نداء معرفة من قبل المستخدم تُستخدم للحصول على تدفق إخراج لكل صفحة مُصوَّرة. |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


يضبط قائمة بأرقام الصفحات لحفظها عند حفظ تخطيط المشروع إلى ملفات منفصلة.

--------------------

سيتم حفظ جميع الصفحات إذا كانت هذه القائمة فارغة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.List&lt;java.lang.Integer&gt; | قائمة بأرقام الصفحات لحفظها عند حفظ تخطيط المشروع في ملفات منفصلة. |

### setPixelFormat(int value) {#setPixelFormat-int-}
```
public final void setPixelFormat(int value)
```


يضبط تنسيق بيانات اللون لكل بكسل في الصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | تنسيق بيانات اللون لكل بكسل في الصورة. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب تقليل الفجوة بين المهمة الأخيرة وتذييل الصفحة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب تقليل الفجوة بين آخر مهمة وتذييل الصفحة. |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


يضبط نوع الضغط الذي يُطبق عند حفظ الصور المولدة بتنسيق TIFF.

--------------------

يؤثر فقط عند الحفظ إلى TIFF. القيمة الافتراضية هي `TiffCompressionLZW`([getTiffCompression()](../../com.aspose.tasks/imagesaveoptions\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\#setTiffCompression-int-)).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | نوع الضغط الذي يُطبق عند حفظ الصور المولدة بصيغة TIFF. |

### setVerticalResolution(float value) {#setVerticalResolution-float-}
```
public final void setVerticalResolution(float value)
```


يضبط الدقة العمودية بوحدة dpi.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float | دقة العمودية بوحدة dpi. |

