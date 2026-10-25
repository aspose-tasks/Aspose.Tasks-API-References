---
title: "XpsOptions"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Proje sayfalarını XPS'e render ederken ek seçenekleri belirtmeye izin verir."
type: docs
weight: 369
url: /tr/java/com.aspose.tasks/xpsoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.ICloneableSaveOptions
```
public class XpsOptions extends SaveOptions implements ICloneableSaveOptions
```

Proje sayfalarını XPS'e render ederken ek seçenekleri belirtmeye izin verir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [XpsOptions()](#XpsOptions--) | Yeni bir [XpsOptions](../../com.aspose.tasks/xpsoptions) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getRenderMetafileAsBitmap()](#getRenderMetafileAsBitmap--) | Bir metafilenin bitmap olarak işlenip işlenmeyeceğini gösteren bir değeri alır. |
| [setRenderMetafileAsBitmap(boolean value)](#setRenderMetafileAsBitmap-boolean-) | Bir metafilenin bitmap olarak işlenip işlenmeyeceğini gösteren bir değeri ayarlar. |
### XpsOptions() {#XpsOptions--}
```
public XpsOptions()
```


Yeni bir [XpsOptions](../../com.aspose.tasks/xpsoptions) sınıfı örneği başlatır.

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
### getRenderMetafileAsBitmap() {#getRenderMetafileAsBitmap--}
```
public final boolean getRenderMetafileAsBitmap()
```


Bir metafilenin bitmap olarak işlenip işlenmeyeceğini gösteren bir değeri alır.

**Returns:**
boolean - bir metafilenin bitmap olarak işlenip işlenmeyeceğini gösteren değer.
### setRenderMetafileAsBitmap(boolean value) {#setRenderMetafileAsBitmap-boolean-}
```
public final void setRenderMetafileAsBitmap(boolean value)
```


Bir metafilenin bitmap olarak işlenip işlenmeyeceğini gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | bir metafilenin bitmap olarak işlenip işlenmeyeceğini gösteren değer. |

