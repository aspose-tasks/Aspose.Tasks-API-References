---
title: "FontSettings"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يحدد إعدادات الخط المستخدمة عند عرض المشاريع."
type: docs
weight: 101
url: /ar/java/com.aspose.tasks/fontsettings/
---

**Inheritance:**
java.lang.Object
```
public final class FontSettings
```

يحدد إعدادات الخط المستخدمة عند عرض رؤية المشروع.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [FontSettings()](#FontSettings--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getDefaultFontName()](#getDefaultFontName--) | يحصل على الخط الافتراضي (أو الاحتياطي) للعرض. |
| [getFontResolveCallback()](#getFontResolveCallback--) | يحصل على رد نداء يمكن استخدامه لتخصيص الخطوط المحلولة. |
| [getUseProjectDefaultFont()](#getUseProjectDefaultFont--) | يحصل على قيمة تشير إلى ما إذا كان يجب استخدام الخط الافتراضي للعرض. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | يضبط الخط الافتراضي (أو الاحتياطي) للعرض. |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | يضبط المجلدات التي يبحث فيها Aspose.Tasks عن خطوط TrueType عند عرض المشروع. |
| [setFontResolveCallback(FontResolveCallbackDelegate value)](#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-) | يضبط رد نداء يمكن استخدامه لتخصيص الخطوط المحلولة. |
| [setUseProjectDefaultFont(boolean value)](#setUseProjectDefaultFont-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب استخدام الخط الافتراضي للعرض. |
### FontSettings() {#FontSettings--}
```
public FontSettings()
```


### getDefaultFontName() {#getDefaultFontName--}
```
public final String getDefaultFontName()
```


يحصل على الخط الافتراضي (أو الاحتياطي) للعرض.

**Returns:**
java.lang.String - الخط الافتراضي (أو الاحتياطي) للعرض.
### getFontResolveCallback() {#getFontResolveCallback--}
```
public final FontResolveCallbackDelegate getFontResolveCallback()
```


يحصل على رد نداء يمكن استخدامه لتخصيص الخطوط المحلولة.

**Returns:**
[FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) - a callback which can be used to customize resolved fonts.
### getUseProjectDefaultFont() {#getUseProjectDefaultFont--}
```
public final boolean getUseProjectDefaultFont()
```


يحصل على قيمة تشير إلى ما إذا كان يجب استخدام الخط الافتراضي للعرض.

--------------------

عند كون القيمة False وتحديد DefaultFontName، سيستخدم محرك العرض الخط المحدد بواسطة DefaultFontName كخط احتياطي. وإلا يتم استخدام خط 'Arial' (إذا كان مثبتًا) أو خطوط 'Generic Sans Serif' كخط احتياطي. يُستَخدم الخط الاحتياطي أثناء عرض مشروع عندما يشير نمط النص إلى خط غير مثبت على نظام التشغيل الحالي. للحصول على تحكم أكبر في حل الخطوط يمكنك استخدام `FontResolveCallback`([getFontResolveCallback](../../com.aspose.tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose.tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-)) رد الاتصال.

**Returns:**
منطقي - قيمة تشير إلى ما إذا كان يجب استخدام الخط الافتراضي في العرض.
### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public final void setDefaultFontName(String value)
```


يضبط الخط الافتراضي (أو الاحتياطي) للعرض.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | الخط الافتراضي (أو الاحتياطي) للعرض. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public final void setFontFolders(String[] fontFolders, boolean recursive)
```


يضبط المجلدات التي يبحث فيها Aspose.Tasks عن خطوط TrueType عند عرض المشروع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fontFolders | java.lang.String[] | مصفوفة من المجلدات التي تحتوي على خطوط TrueType. |
| recursive | منطقي | إذا كان True سيتم فحص المجلدات المحددة بشكل متكرر. |

### setFontResolveCallback(FontResolveCallbackDelegate value) {#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-}
```
public final void setFontResolveCallback(FontResolveCallbackDelegate value)
```


يضبط رد نداء يمكن استخدامه لتخصيص الخطوط المحلولة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) | رد اتصال يمكن استخدامه لتخصيص الخطوط التي تم حلها. |

### setUseProjectDefaultFont(boolean value) {#setUseProjectDefaultFont-boolean-}
```
public final void setUseProjectDefaultFont(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب استخدام الخط الافتراضي للعرض.

--------------------

عند كون القيمة False وتحديد DefaultFontName، سيستخدم محرك العرض الخط المحدد بواسطة DefaultFontName كخط احتياطي. وإلا يتم استخدام خط 'Arial' (إذا كان مثبتًا) أو خطوط 'Generic Sans Serif' كخط احتياطي. يُستَخدم الخط الاحتياطي أثناء عرض مشروع عندما يشير نمط النص إلى خط غير مثبت على نظام التشغيل الحالي. للحصول على تحكم أكبر في حل الخطوط يمكنك استخدام `FontResolveCallback`([getFontResolveCallback](../../com.aspose.tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose.tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-)) رد الاتصال.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب استخدام الخط الافتراضي في العرض. |

