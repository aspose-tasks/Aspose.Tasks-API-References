---
title: "HtmlSaveOptions"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يسمح بتحديد خيارات إضافية عند تحويل صفحات المشروع إلى HTML."
type: docs
weight: 132
url: /ar/java/com.aspose.tasks/htmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class HtmlSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

يسمح بتحديد خيارات إضافية عند تحويل صفحات المشروع إلى HTML.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [HtmlSaveOptions()](#HtmlSaveOptions--) | ينشئ مثيلاً جديدًا من الفئة [HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getCssSavingCallback()](#getCssSavingCallback--) | يحصل على رد النداء الذي يُستدعى لإنشاء مورد لتخزين CSS. |
| [getCssStylePrefix()](#getCssStylePrefix--) | يحصل على بادئة نمط CSS. |
| [getExportCss()](#getExportCss--) | يحصل على طريقة تصدير CSS. |
| [getExportFonts()](#getExportFonts--) | يحصل على طريقة تصدير الخطوط. |
| [getExportImages()](#getExportImages--) | يحصل على طريقة تصدير الصور. |
| [getFontFaceTypes()](#getFontFaceTypes--) | يحصل على أنواع خطوط الواجهة. |
| [getFontSavingCallback()](#getFontSavingCallback--) | يحصل على رد النداء الذي يُستدعى لإنشاء مورد لتخزين الخط. |
| [getFontSettings()](#getFontSettings--) | يحدد إعدادات الخط المستخدمة عند عرض رؤية المشروع. |
| [getImageSavingCallback()](#getImageSavingCallback--) | يحصل على رد النداء الذي يُستدعى لإنشاء مورد لتخزين الخط. |
| [getIncludeProjectNameInPageHeader()](#getIncludeProjectNameInPageHeader--) | يحصل على قيمة تشير إلى ما إذا كان يجب تضمين اسم المشروع في رأس صفحة HTML. |
| [getIncludeProjectNameInTitle()](#getIncludeProjectNameInTitle--) | يحصل على قيمة تشير إلى ما إذا كان يجب تضمين اسم المشروع في عنوان HTML. |
| [getPageSavingCallback()](#getPageSavingCallback--) | يحصل على رد نداء معرف من قبل المستخدم يُستخدم للحصول على تدفق إخراج لكل صفحة مُعالجة. |
| [getPages()](#getPages--) | يحصل على قائمة بأرقام الصفحات التي يجب حفظها عند معالجة تخطيط المشروع. |
| [getReduceFooterGap()](#getReduceFooterGap--) | يحصل على قيمة تشير إلى ما إذا كان يجب تقليل الفجوة بين المهمة الأخيرة وتذييل الصفحة. |
| [getUseGradientBrush()](#getUseGradientBrush--) | يحصل على قيمة تشير إلى ما إذا كان يجب استخدام فرشاة تدرجية عند معالجة تخطيط المشروع. |
| [setCssSavingCallback(ICssSavingCallback value)](#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-) | يضبط رد النداء الذي يُستدعى لإنشاء مورد لتخزين CSS. |
| [setCssStylePrefix(String value)](#setCssStylePrefix-java.lang.String-) | يضبط بادئة نمط CSS. |
| [setExportCss(int value)](#setExportCss-int-) | يضبط طريقة تصدير CSS. |
| [setExportFonts(int value)](#setExportFonts-int-) | يضبط طريقة تصدير الخطوط. |
| [setExportImages(int value)](#setExportImages-int-) | يضبط طريقة تصدير الصور. |
| [setFontFaceTypes(int value)](#setFontFaceTypes-int-) | يضبط أنواع واجهة الخط. |
| [setFontSavingCallback(IFontSavingCallback value)](#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-) | يضبط رد النداء الذي يُستدعى لإنشاء مورد لتخزين الخط. |
| [setImageSavingCallback(IImageSavingCallback value)](#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-) | يضبط رد النداء الذي يُستدعى لإنشاء مورد لتخزين الخط. |
| [setIncludeProjectNameInPageHeader(boolean value)](#setIncludeProjectNameInPageHeader-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب تضمين اسم المشروع في رأس صفحة HTML. |
| [setIncludeProjectNameInTitle(boolean value)](#setIncludeProjectNameInTitle-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب تضمين اسم المشروع في عنوان HTML. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | يضبط رد نداء معرف من قبل المستخدم يُستخدم للحصول على تدفق إخراج لكل صفحة مُعالجة. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | يضبط قائمة أرقام الصفحات التي يجب حفظها عند معالجة تخطيط المشروع. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب تقليل الفجوة بين المهمة الأخيرة وتذييل الصفحة. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب استخدام فرشاة تدرجية عند معالجة تخطيط المشروع. |
### HtmlSaveOptions() {#HtmlSaveOptions--}
```
public HtmlSaveOptions()
```


ينشئ مثيلاً جديدًا من الفئة [HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions).

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
### getCssSavingCallback() {#getCssSavingCallback--}
```
public final ICssSavingCallback getCssSavingCallback()
```


يحصل على رد النداء الذي يُستدعى لإنشاء مورد لتخزين CSS.

**Returns:**
[ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) - the callback that is called to create resource to store CSS.
### getCssStylePrefix() {#getCssStylePrefix--}
```
public final String getCssStylePrefix()
```


يحصل على بادئة نمط CSS.

**Returns:**
java.lang.String - بادئة نمط CSS.
### getExportCss() {#getExportCss--}
```
public final int getExportCss()
```


يحصل على طريقة تصدير CSS.

**Returns:**
int - طريقة تصدير CSS.
### getExportFonts() {#getExportFonts--}
```
public final int getExportFonts()
```


يحصل على طريقة تصدير الخطوط.

**Returns:**
int - طريقة تصدير الخطوط.
### getExportImages() {#getExportImages--}
```
public final int getExportImages()
```


يحصل على طريقة تصدير الصور.

**Returns:**
int - طريقة تصدير الصور.
### getFontFaceTypes() {#getFontFaceTypes--}
```
public final int getFontFaceTypes()
```


يحصل على أنواع خطوط الواجهة.

القيمة: أنواع واجهة الخط.

**Returns:**
int - أنواع واجهة الخط.
### getFontSavingCallback() {#getFontSavingCallback--}
```
public final IFontSavingCallback getFontSavingCallback()
```


يحصل على رد النداء الذي يُستدعى لإنشاء مورد لتخزين الخط.

**Returns:**
[IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) - the callback that is called to create resource to store font.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


يحدد إعدادات الخط المستخدمة عند عرض رؤية المشروع.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getImageSavingCallback() {#getImageSavingCallback--}
```
public final IImageSavingCallback getImageSavingCallback()
```


يحصل على رد النداء الذي يُستدعى لإنشاء مورد لتخزين الخط.

**Returns:**
[IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) - the callback that is called to create resource to store font.
### getIncludeProjectNameInPageHeader() {#getIncludeProjectNameInPageHeader--}
```
public final boolean getIncludeProjectNameInPageHeader()
```


يحصل على قيمة تشير إلى ما إذا كان يجب تضمين اسم المشروع في رأس صفحة HTML.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب تضمين اسم المشروع في رأس صفحة HTML.
### getIncludeProjectNameInTitle() {#getIncludeProjectNameInTitle--}
```
public final boolean getIncludeProjectNameInTitle()
```


يحصل على قيمة تشير إلى ما إذا كان يجب تضمين اسم المشروع في عنوان HTML.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب تضمين اسم المشروع في عنوان HTML.
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


يحصل على قائمة بأرقام الصفحات التي يجب حفظها عند معالجة تخطيط المشروع.

--------------------

سيتم حفظ جميع صفحات المشروع إذا كانت هذه القائمة فارغة.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - قائمة أرقام الصفحات التي يجب حفظها عند معالجة تخطيط المشروع.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


يحصل على قيمة تشير إلى ما إذا كان يجب تقليل الفجوة بين المهمة الأخيرة وتذييل الصفحة.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب تقليل الفجوة بين المهمة الأخيرة وتذييل الصفحة.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


يحصل على قيمة تشير إلى ما إذا كان يجب استخدام فرشاة تدرجية عند معالجة تخطيط المشروع.

--------------------

استخدام الفرشاة التدرجية حاليًا غير مدعوم عند المعالجة إلى HTML.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب استخدام فرشاة تدرجية عند معالجة تخطيط المشروع.
### setCssSavingCallback(ICssSavingCallback value) {#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-}
```
public final void setCssSavingCallback(ICssSavingCallback value)
```


يضبط رد النداء الذي يُستدعى لإنشاء مورد لتخزين CSS.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) | رد النداء الذي يُستدعى لإنشاء مورد لتخزين CSS. |

### setCssStylePrefix(String value) {#setCssStylePrefix-java.lang.String-}
```
public final void setCssStylePrefix(String value)
```


يضبط بادئة نمط CSS.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | بادئة نمط CSS. |

### setExportCss(int value) {#setExportCss-int-}
```
public final void setExportCss(int value)
```


يضبط طريقة تصدير CSS.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | طريقة تصدير CSS. |

### setExportFonts(int value) {#setExportFonts-int-}
```
public final void setExportFonts(int value)
```


يضبط طريقة تصدير الخطوط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | طريقة تصدير الخطوط. |

### setExportImages(int value) {#setExportImages-int-}
```
public final void setExportImages(int value)
```


يضبط طريقة تصدير الصور.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | طريقة تصدير الصور. |

### setFontFaceTypes(int value) {#setFontFaceTypes-int-}
```
public final void setFontFaceTypes(int value)
```


يضبط أنواع واجهة الخط.

القيمة: أنواع واجهة الخط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | أنواع خطوط الوجه. |

### setFontSavingCallback(IFontSavingCallback value) {#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-}
```
public final void setFontSavingCallback(IFontSavingCallback value)
```


يضبط رد النداء الذي يُستدعى لإنشاء مورد لتخزين الخط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) | الدالة الراجعة التي تُستدعى لإنشاء مورد لتخزين الخط. |

### setImageSavingCallback(IImageSavingCallback value) {#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-}
```
public final void setImageSavingCallback(IImageSavingCallback value)
```


يضبط رد النداء الذي يُستدعى لإنشاء مورد لتخزين الخط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) | الدالة الراجعة التي تُستدعى لإنشاء مورد لتخزين الخط. |

### setIncludeProjectNameInPageHeader(boolean value) {#setIncludeProjectNameInPageHeader-boolean-}
```
public final void setIncludeProjectNameInPageHeader(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب تضمين اسم المشروع في رأس صفحة HTML.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب تضمين اسم المشروع في رأس صفحة HTML. |

### setIncludeProjectNameInTitle(boolean value) {#setIncludeProjectNameInTitle-boolean-}
```
public final void setIncludeProjectNameInTitle(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب تضمين اسم المشروع في عنوان HTML.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب تضمين اسم المشروع في عنوان HTML. |

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


يضبط قائمة أرقام الصفحات التي يجب حفظها عند معالجة تخطيط المشروع.

--------------------

سيتم حفظ جميع صفحات المشروع إذا كانت هذه القائمة فارغة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.List&lt;java.lang.Integer&gt; | قائمة بأرقام الصفحات التي يجب حفظها عند تصيير تخطيط المشروع. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب تقليل الفجوة بين المهمة الأخيرة وتذييل الصفحة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب تقليل الفجوة بين آخر مهمة وتذييل الصفحة. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب استخدام فرشاة تدرجية عند معالجة تخطيط المشروع.

--------------------

استخدام الفرشاة التدرجية حاليًا غير مدعوم عند المعالجة إلى HTML.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب استخدام فرشاة التدرج عند تصيير تخطيط المشروع. |

