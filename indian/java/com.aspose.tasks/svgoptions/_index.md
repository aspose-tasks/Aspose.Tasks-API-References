---
title: "SvgOptions"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "प्रोजेक्ट पृष्ठों को SVG में रेंडर करते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।"
type: docs
weight: 283
url: /hi/java/com.aspose.tasks/svgoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.ICloneableSaveOptions
```
public class SvgOptions extends SaveOptions implements ICloneableSaveOptions
```

प्रोजेक्ट पृष्ठों को SVG में रेंडर करते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [SvgOptions()](#SvgOptions--) | एक नया [SvgOptions](../../com.aspose.tasks/svgoptions) क्लास का इंस्टेंस इनिशियलाइज़ करता है जिसका उपयोग प्रोजेक्ट को SVG फ़ॉर्मेट में सहेजने के लिए किया जा सकता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getPageSavingCallback()](#getPageSavingCallback--) | एक उपयोगकर्ता-परिभाषित इम्प्लीमेंटेशन कॉलबैक प्राप्त करता है जिसका उपयोग प्रत्येक रेंडर किए गए पेज के लिए आउटपुट स्ट्रीम प्राप्त करने में किया जाता है। |
| [getUseGradientBrush()](#getUseGradientBrush--) | निर्धारित करता है कि प्रोजेक्ट लेआउट के रेंडरिंग के समय ग्रेडिएंट ब्रश का उपयोग किया जाए या नहीं। |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | एक उपयोगकर्ता-परिभाषित इम्प्लीमेंटेशन कॉलबैक सेट करता है जिसका उपयोग प्रत्येक रेंडर किए गए पेज के लिए आउटपुट स्ट्रीम प्राप्त करने में किया जाता है। |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | निर्धारित करता है कि प्रोजेक्ट लेआउट के रेंडरिंग के समय ग्रेडिएंट ब्रश का उपयोग किया जाए या नहीं। |
### SvgOptions() {#SvgOptions--}
```
public SvgOptions()
```


एक नया [SvgOptions](../../com.aspose.tasks/svgoptions) क्लास का इंस्टेंस इनिशियलाइज़ करता है जिसका उपयोग प्रोजेक्ट को SVG फ़ॉर्मेट में सहेजने के लिए किया जा सकता है।

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
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


एक उपयोगकर्ता-परिभाषित इम्प्लीमेंटेशन कॉलबैक प्राप्त करता है जिसका उपयोग प्रत्येक रेंडर किए गए पेज के लिए आउटपुट स्ट्रीम प्राप्त करने में किया जाता है।

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined implementation callback which is used to get an output stream for each rendered page.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


निर्धारित करता है कि प्रोजेक्ट लेआउट के रेंडरिंग के समय ग्रेडिएंट ब्रश का उपयोग किया जाए या नहीं।

--------------------

वर्तमान में SVG में रेंडरिंग के लिए ग्रेडिएंट ब्रश का उपयोग समर्थित नहीं है।

**Returns:**
boolean - एक मान जो दर्शाता है कि प्रोजेक्ट लेआउट के रेंडरिंग के समय ग्रेडिएंट ब्रश का उपयोग किया जाए या नहीं।
### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


एक उपयोगकर्ता-परिभाषित इम्प्लीमेंटेशन कॉलबैक सेट करता है जिसका उपयोग प्रत्येक रेंडर किए गए पेज के लिए आउटपुट स्ट्रीम प्राप्त करने में किया जाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | एक उपयोगकर्ता-परिभाषित इम्प्लीमेंटेशन कॉलबैक जो प्रत्येक रेंडर किए गए पेज के लिए आउटपुट स्ट्रीम प्राप्त करने में उपयोग किया जाता है। |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


निर्धारित करता है कि प्रोजेक्ट लेआउट के रेंडरिंग के समय ग्रेडिएंट ब्रश का उपयोग किया जाए या नहीं।

--------------------

वर्तमान में SVG में रेंडरिंग के लिए ग्रेडिएंट ब्रश का उपयोग समर्थित नहीं है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि प्रोजेक्ट लेआउट के रेंडरिंग के समय ग्रेडिएंट ब्रश का उपयोग किया जाए या नहीं। |

