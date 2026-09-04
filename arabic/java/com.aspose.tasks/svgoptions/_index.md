---
title: "SvgOptions"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يسمح بتحديد خيارات إضافية عند تصيير صفحات المشروع إلى SVG."
type: docs
weight: 283
url: /ar/java/com.aspose.tasks/svgoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.ICloneableSaveOptions
```
public class SvgOptions extends SaveOptions implements ICloneableSaveOptions
```

يسمح بتحديد خيارات إضافية عند تصيير صفحات المشروع إلى SVG.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [SvgOptions()](#SvgOptions--) | ينشئ مثلاً جديدًا من الفئة [SvgOptions](../../com.aspose.tasks/svgoptions) التي يمكن استخدامها لحفظ المشروع بتنسيق SVG. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getPageSavingCallback()](#getPageSavingCallback--) | يحصل على رد اتصال تنفيذ معرف من قبل المستخدم يُستخدم للحصول على تدفق إخراج لكل صفحة مُعروضة. |
| [getUseGradientBrush()](#getUseGradientBrush--) | يحدد ما إذا كان يجب استخدام فرشاة تدرجية عند عرض تخطيط المشروع. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | يضبط رد اتصال تنفيذ معرف من قبل المستخدم يُستخدم للحصول على تدفق إخراج لكل صفحة مُعروضة. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | يحدد ما إذا كان يجب استخدام فرشاة تدرجية عند عرض تخطيط المشروع. |
### SvgOptions() {#SvgOptions--}
```
public SvgOptions()
```


ينشئ مثلاً جديدًا من الفئة [SvgOptions](../../com.aspose.tasks/svgoptions) التي يمكن استخدامها لحفظ المشروع بتنسيق SVG.

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
public final SaveOptions deepClone()
```


محجوز للاستخدام الداخلي.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


يحصل على رد اتصال تنفيذ معرف من قبل المستخدم يُستخدم للحصول على تدفق إخراج لكل صفحة مُعروضة.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined implementation callback which is used to get an output stream for each rendered page.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


يحدد ما إذا كان يجب استخدام فرشاة تدرجية عند عرض تخطيط المشروع.

--------------------

حاليًا لا يُدعم استخدام الفرشاة التدرجية في العرض إلى SVG.

**Returns:**
منطقي - قيمة تشير إلى ما إذا كان يجب استخدام فرشاة تدرجية عند عرض تخطيط المشروع.
### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


يضبط رد اتصال تنفيذ معرف من قبل المستخدم يُستخدم للحصول على تدفق إخراج لكل صفحة مُعروضة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | رد اتصال تنفيذ معرف من قبل المستخدم يُستخدم للحصول على تدفق إخراج لكل صفحة مُعروضة. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


يحدد ما إذا كان يجب استخدام فرشاة تدرجية عند عرض تخطيط المشروع.

--------------------

حاليًا لا يُدعم استخدام الفرشاة التدرجية في العرض إلى SVG.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب استخدام فرشاة تدرجية عند عرض تخطيط المشروع. |

