---
title: "XpsOptions"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "प्रोजेक्ट पेजों को XPS में रेंडर करते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।"
type: docs
weight: 369
url: /hi/java/com.aspose.tasks/xpsoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.ICloneableSaveOptions
```
public class XpsOptions extends SaveOptions implements ICloneableSaveOptions
```

प्रोजेक्ट पेजों को XPS में रेंडर करते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [XpsOptions()](#XpsOptions--) | एक नया उदाहरण प्रारंभ करता है [XpsOptions](../../com.aspose.tasks/xpsoptions) वर्ग का। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getRenderMetafileAsBitmap()](#getRenderMetafileAsBitmap--) | एक मान प्राप्त करता है जो दर्शाता है कि क्या एक मेटाफाइल को बिटमैप के रूप में रेंडर किया जाना चाहिए। |
| [setRenderMetafileAsBitmap(boolean value)](#setRenderMetafileAsBitmap-boolean-) | एक मान सेट करता है जो दर्शाता है कि क्या एक मेटाफाइल को बिटमैप के रूप में रेंडर किया जाना चाहिए। |
### XpsOptions() {#XpsOptions--}
```
public XpsOptions()
```


एक नया उदाहरण प्रारंभ करता है [XpsOptions](../../com.aspose.tasks/xpsoptions) वर्ग का।

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public final void copyOutputPropertiesFrom(SaveOptions source)
```


आंतरिक उपयोग के लिए आरक्षित।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| source | [SaveOptions](../../com.aspose.tasks/saveoptions) | \{@inheritDoc\} |

### deepClone() {#deepClone--}
```
public final SaveOptions deepClone()
```


आंतरिक उपयोग के लिए आरक्षित।

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getRenderMetafileAsBitmap() {#getRenderMetafileAsBitmap--}
```
public final boolean getRenderMetafileAsBitmap()
```


एक मान प्राप्त करता है जो दर्शाता है कि क्या एक मेटाफाइल को बिटमैप के रूप में रेंडर किया जाना चाहिए।

**Returns:**
boolean - एक मान जो दर्शाता है कि क्या एक मेटाफाइल को बिटमैप के रूप में रेंडर किया जाना चाहिए।
### setRenderMetafileAsBitmap(boolean value) {#setRenderMetafileAsBitmap-boolean-}
```
public final void setRenderMetafileAsBitmap(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि क्या एक मेटाफाइल को बिटमैप के रूप में रेंडर किया जाना चाहिए।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि क्या एक मेटाफाइल को बिटमैप के रूप में रेंडर किया जाना चाहिए। |

