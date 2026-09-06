---
title: "SvgOptions"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Proje sayfalarını SVG'ye render ederken ek seçenekler belirtmeye izin verir."
type: docs
weight: 283
url: /tr/java/com.aspose.tasks/svgoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.ICloneableSaveOptions
```
public class SvgOptions extends SaveOptions implements ICloneableSaveOptions
```

Proje sayfalarını SVG'ye render ederken ek seçenekler belirtmeye izin verir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [SvgOptions()](#SvgOptions--) | Projeyi SVG formatında kaydetmek için kullanılabilecek [SvgOptions](../../com.aspose.tasks/svgoptions) sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getPageSavingCallback()](#getPageSavingCallback--) | Her render edilen sayfa için bir çıktı akışı elde etmek üzere kullanılan kullanıcı tanımlı uygulama geri çağrısını alır. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Proje düzeni render edilirken degrade fırçasının kullanılıp kullanılmayacağını belirler. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Her render edilen sayfa için bir çıktı akışı elde etmek üzere kullanılan kullanıcı tanımlı uygulama geri çağrısını ayarlar. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Proje düzeni render edilirken degrade fırçasının kullanılıp kullanılmayacağını belirler. |
### SvgOptions() {#SvgOptions--}
```
public SvgOptions()
```


Projeyi SVG formatında kaydetmek için kullanılabilecek [SvgOptions](../../com.aspose.tasks/svgoptions) sınıfının yeni bir örneğini başlatır.

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public final void copyOutputPropertiesFrom(SaveOptions source)
```


Dahili kullanım için ayrılmıştır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | [SaveOptions](../../com.aspose.tasks/saveoptions) | \{@inheritDoc\} |

### deepClone() {#deepClone--}
```
public final SaveOptions deepClone()
```


Dahili kullanım için ayrılmıştır.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Her render edilen sayfa için bir çıktı akışı elde etmek üzere kullanılan kullanıcı tanımlı uygulama geri çağrısını alır.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined implementation callback which is used to get an output stream for each rendered page.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Proje düzeni render edilirken degrade fırçasının kullanılıp kullanılmayacağını belirler.

--------------------

Şu anda degrade fırçasının SVG'ye render edilmesi desteklenmemektedir.

**Returns:**
boolean - proje düzeni render edilirken degrade fırçasının kullanılıp kullanılmayacağını gösteren değer.
### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Her render edilen sayfa için bir çıktı akışı elde etmek üzere kullanılan kullanıcı tanımlı uygulama geri çağrısını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | Her render edilen sayfa için bir çıktı akışı elde etmek üzere kullanılan kullanıcı tanımlı uygulama geri çağrısı. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Proje düzeni render edilirken degrade fırçasının kullanılıp kullanılmayacağını belirler.

--------------------

Şu anda degrade fırçasının SVG'ye render edilmesi desteklenmemektedir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | proje düzeni render edilirken degrade fırçasının kullanılıp kullanılmayacağını gösteren değer. |

