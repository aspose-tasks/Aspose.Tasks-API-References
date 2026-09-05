---
title: "FontSettings"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "प्रोजेक्ट व्यू को रेंडर करते समय उपयोग किए जाने वाले फ़ॉन्ट सेटिंग्स को निर्दिष्ट करता है।"
type: docs
weight: 101
url: /hi/java/com.aspose.tasks/fontsettings/
---

**Inheritance:**
java.lang.Object
```
public final class FontSettings
```

प्रोजेक्ट के दृश्य को रेंडर करते समय उपयोग किए जाने वाले फ़ॉन्ट सेटिंग्स को निर्दिष्ट करता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [FontSettings()](#FontSettings--) |  |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getDefaultFontName()](#getDefaultFontName--) | रेंडरिंग के लिए डिफ़ॉल्ट (या फॉलबैक) फ़ॉन्ट प्राप्त करता है। |
| [getFontResolveCallback()](#getFontResolveCallback--) | एक कॉलबैक प्राप्त करता है जिसका उपयोग हल किए गए फ़ॉन्ट को अनुकूलित करने के लिए किया जा सकता है। |
| [getUseProjectDefaultFont()](#getUseProjectDefaultFont--) | एक मान प्राप्त करता है जो दर्शाता है कि रेंडरिंग के लिए डिफ़ॉल्ट फ़ॉन्ट का उपयोग अनिवार्य है या नहीं। |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | रेंडरिंग के लिए डिफ़ॉल्ट (या फॉलबैक) फ़ॉन्ट सेट करता है। |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Aspose.Tasks उन फ़ोल्डरों को सेट करता है जहाँ प्रोजेक्ट के व्यू को रेंडर करते समय TrueType फ़ॉन्ट खोजे जाते हैं। |
| [setFontResolveCallback(FontResolveCallbackDelegate value)](#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-) | एक कॉलबैक सेट करता है जिसका उपयोग हल किए गए फ़ॉन्ट को अनुकूलित करने के लिए किया जा सकता है। |
| [setUseProjectDefaultFont(boolean value)](#setUseProjectDefaultFont-boolean-) | एक मान सेट करता है जो दर्शाता है कि रेंडरिंग के लिए डिफ़ॉल्ट फ़ॉन्ट का उपयोग अनिवार्य है या नहीं। |
### FontSettings() {#FontSettings--}
```
public FontSettings()
```


### getDefaultFontName() {#getDefaultFontName--}
```
public final String getDefaultFontName()
```


रेंडरिंग के लिए डिफ़ॉल्ट (या फॉलबैक) फ़ॉन्ट प्राप्त करता है।

**Returns:**
java.lang.String - रेंडरिंग के लिए डिफ़ॉल्ट (या फॉलबैक) फ़ॉन्ट।
### getFontResolveCallback() {#getFontResolveCallback--}
```
public final FontResolveCallbackDelegate getFontResolveCallback()
```


एक कॉलबैक प्राप्त करता है जिसका उपयोग हल किए गए फ़ॉन्ट को अनुकूलित करने के लिए किया जा सकता है।

**Returns:**
[FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) - a callback which can be used to customize resolved fonts.
### getUseProjectDefaultFont() {#getUseProjectDefaultFont--}
```
public final boolean getUseProjectDefaultFont()
```


एक मान प्राप्त करता है जो दर्शाता है कि रेंडरिंग के लिए डिफ़ॉल्ट फ़ॉन्ट का उपयोग अनिवार्य है या नहीं।

--------------------

जब मान False हो और DefaultFontName निर्दिष्ट किया गया हो, तो रेंडरिंग इंजन DefaultFontName द्वारा निर्दिष्ट फ़ॉन्ट को फ़ॉलबैक फ़ॉन्ट के रूप में उपयोग करेगा। अन्यथा 'Arial' (यदि स्थापित है) या 'Generic Sans Serif' फ़ॉन्ट को फ़ॉलबैक फ़ॉन्ट के रूप में उपयोग किया जाता है। फ़ॉलबैक फ़ॉन्ट प्रोजेक्ट व्यू के रेंडरिंग के दौरान उपयोग किया जाता है जब कोई टेक्स्ट स्टाइल ऐसे फ़ॉन्ट का संदर्भ देता है जो वर्तमान ऑपरेटिंग सिस्टम में स्थापित नहीं है। फ़ॉन्ट रिज़ॉल्यूशन पर अधिक नियंत्रण के लिए आप `FontResolveCallback`([getFontResolveCallback](../../com.aspose.tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose.tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-)) कॉलबैक का उपयोग कर सकते हैं।

**Returns:**
boolean - एक मान जो दर्शाता है कि रेंडरिंग के लिए डिफ़ॉल्ट फ़ॉन्ट का उपयोग किया जाना चाहिए या नहीं।
### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public final void setDefaultFontName(String value)
```


रेंडरिंग के लिए डिफ़ॉल्ट (या फॉलबैक) फ़ॉन्ट सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | रेंडरिंग के लिए डिफ़ॉल्ट (या फ़ॉलबैक) फ़ॉन्ट। |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public final void setFontFolders(String[] fontFolders, boolean recursive)
```


Aspose.Tasks उन फ़ोल्डरों को सेट करता है जहाँ प्रोजेक्ट के व्यू को रेंडर करते समय TrueType फ़ॉन्ट खोजे जाते हैं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fontFolders | java.lang.String[] | TrueType फ़ॉन्ट्स वाले फ़ोल्डरों की एक एरे। |
| recursive | boolean | यदि true हो तो निर्दिष्ट फ़ोल्डरों को पुनरावर्ती रूप से स्कैन किया जाएगा। |

### setFontResolveCallback(FontResolveCallbackDelegate value) {#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-}
```
public final void setFontResolveCallback(FontResolveCallbackDelegate value)
```


एक कॉलबैक सेट करता है जिसका उपयोग हल किए गए फ़ॉन्ट को अनुकूलित करने के लिए किया जा सकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) | एक कॉलबैक जिसका उपयोग हल किए गए फ़ॉन्ट्स को अनुकूलित करने के लिए किया जा सकता है। |

### setUseProjectDefaultFont(boolean value) {#setUseProjectDefaultFont-boolean-}
```
public final void setUseProjectDefaultFont(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि रेंडरिंग के लिए डिफ़ॉल्ट फ़ॉन्ट का उपयोग अनिवार्य है या नहीं।

--------------------

जब मान False हो और DefaultFontName निर्दिष्ट किया गया हो, तो रेंडरिंग इंजन DefaultFontName द्वारा निर्दिष्ट फ़ॉन्ट को फ़ॉलबैक फ़ॉन्ट के रूप में उपयोग करेगा। अन्यथा 'Arial' (यदि स्थापित है) या 'Generic Sans Serif' फ़ॉन्ट को फ़ॉलबैक फ़ॉन्ट के रूप में उपयोग किया जाता है। फ़ॉलबैक फ़ॉन्ट प्रोजेक्ट व्यू के रेंडरिंग के दौरान उपयोग किया जाता है जब कोई टेक्स्ट स्टाइल ऐसे फ़ॉन्ट का संदर्भ देता है जो वर्तमान ऑपरेटिंग सिस्टम में स्थापित नहीं है। फ़ॉन्ट रिज़ॉल्यूशन पर अधिक नियंत्रण के लिए आप `FontResolveCallback`([getFontResolveCallback](../../com.aspose.tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose.tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-)) कॉलबैक का उपयोग कर सकते हैं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि रेंडरिंग के लिए डिफ़ॉल्ट फ़ॉन्ट का उपयोग किया जाना चाहिए या नहीं। |

