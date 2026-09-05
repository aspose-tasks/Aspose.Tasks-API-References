---
title: "TimescaleTier"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "गैंट चार्ट पर टाइमस्केल की एकल स्तर का प्रतिनिधित्व करता है।"
type: docs
weight: 325
url: /hi/java/com.aspose.tasks/timescaletier/
---

**Inheritance:**
java.lang.Object
```
public final class TimescaleTier
```

गैंट चार्ट पर टाइमस्केल की एकल स्तर का प्रतिनिधित्व करता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [TimescaleTier()](#TimescaleTier--) | नए [TimescaleTier](../../com.aspose.tasks/timescaletier) वर्ग का एक नया उदाहरण प्रारंभ करता है। |
| [TimescaleTier(int unit, int count)](#TimescaleTier-int-int-) | नए [TimescaleTier](../../com.aspose.tasks/timescaletier) वर्ग का एक नया उदाहरण प्रारंभ करता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getAlignment()](#getAlignment--) | टियर के प्रत्येक समय अवधि के भीतर लेबल को कैसे संरेखित किया जाए, प्राप्त करता है ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |
| [getCount()](#getCount--) | टियर के लिए लेबल दिखाने के समय इकाई अंतराल को प्राप्त करता है। |
| [getDateTimeConverter()](#getDateTimeConverter--) | इस टियर में तिथि टिक रेंडरिंग को संभालने के लिए एक कॉलबैक फ़ंक्शन प्राप्त करता है। |
| [getLabel()](#getLabel--) | टाइमस्केल टियर के लिए तिथि लेबल [DateLabel](../../com.aspose.tasks/datelabel) प्राप्त करता है। |
| [getRenderLabelOnEachPage()](#getRenderLabelOnEachPage--) | फ़्लैग प्राप्त करता है जो निर्धारित करता है कि जब एक समय अवधि कई पृष्ठों में फैली हो तो प्रत्येक पृष्ठ पर तिथि लेबल रेंडर किए जाने चाहिए या नहीं। |
| [getShowTicks()](#getShowTicks--) | टियर में समय अवधियों को अलग करने वाले टिक मार्क दिखाने के बारे में संकेत देने वाला मान प्राप्त करता है। |
| [getUnit()](#getUnit--) | टाइमस्केल टियर के लिए टाइमस्केल इकाई [TimescaleUnit](../../com.aspose.tasks/timescaleunit) प्राप्त करता है। |
| [getUsesFiscalYear()](#getUsesFiscalYear--) | टियर लेबल को वित्तीय वर्ष पर आधारित करने के बारे में संकेत देने वाला मान प्राप्त करता है। |
| [setAlignment(int value)](#setAlignment-int-) | टियर के प्रत्येक समय अवधि के भीतर लेबल को कैसे संरेखित किया जाए, सेट करता है ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |
| [setCount(int value)](#setCount-int-) | टियर के लिए लेबल दिखाने के समय इकाई अंतराल को सेट करता है। |
| [setDateTimeConverter(DateTimeConverter value)](#setDateTimeConverter-com.aspose.tasks.DateTimeConverter-) | इस टियर में तिथि टिक रेंडरिंग को संभालने के लिए एक कॉलबैक फ़ंक्शन सेट करता है। |
| [setLabel(int value)](#setLabel-int-) | टाइमस्केल टियर के लिए तिथि लेबल [DateLabel](../../com.aspose.tasks/datelabel) सेट करता है। |
| [setRenderLabelOnEachPage(boolean value)](#setRenderLabelOnEachPage-boolean-) | फ़्लैग सेट करता है जो निर्धारित करता है कि जब एक समय अवधि कई पृष्ठों में फैली हो तो प्रत्येक पृष्ठ पर तिथि लेबल रेंडर किए जाने चाहिए या नहीं। |
| [setShowTicks(boolean value)](#setShowTicks-boolean-) | टियर में समय अवधियों को अलग करने वाले टिक मार्क दिखाने के बारे में संकेत देने वाला मान सेट करता है। |
| [setUnit(int value)](#setUnit-int-) | टाइमस्केल टियर के लिए टाइमस्केल इकाई [TimescaleUnit](../../com.aspose.tasks/timescaleunit) सेट करता है। |
| [setUsesFiscalYear(boolean value)](#setUsesFiscalYear-boolean-) | टियर लेबल को वित्तीय वर्ष पर आधारित करने के बारे में संकेत देने वाला मान सेट करता है। |
### TimescaleTier() {#TimescaleTier--}
```
public TimescaleTier()
```


नए [TimescaleTier](../../com.aspose.tasks/timescaletier) वर्ग का एक नया उदाहरण प्रारंभ करता है।

### TimescaleTier(int unit, int count) {#TimescaleTier-int-int-}
```
public TimescaleTier(int unit, int count)
```


नए [TimescaleTier](../../com.aspose.tasks/timescaletier) वर्ग का एक नया उदाहरण प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| unit | int | टाइमस्केल इकाई [TimescaleUnit](../../com.aspose.tasks/timescaleunit) है। |
| count | int | [TimescaleUnit](../../com.aspose.tasks/timescaleunit) इकाइयों की गिनती। |

### getAlignment() {#getAlignment--}
```
public final int getAlignment()
```


टियर के प्रत्येक समय अवधि के भीतर लेबल को कैसे संरेखित किया जाए, प्राप्त करता है ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).

**Returns:**
int - टियर के प्रत्येक समय अवधि के भीतर लेबल को कैसे संरेखित किया जाए ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).
### getCount() {#getCount--}
```
public final int getCount()
```


टियर के लिए लेबल दिखाने के समय इकाई अंतराल को प्राप्त करता है। डिफ़ॉल्ट मान 1 है।

**Returns:**
int - टियर के लिए लेबल दिखाने के समय इकाई अंतराल।
### getDateTimeConverter() {#getDateTimeConverter--}
```
public final DateTimeConverter getDateTimeConverter()
```


इस टियर में तिथि टिक रेंडरिंग को संभालने के लिए एक कॉलबैक फ़ंक्शन प्राप्त करता है।

**Returns:**
[DateTimeConverter](../../com.aspose.tasks/datetimeconverter) - a callback function for handling rendering date tick in this tier.
### getLabel() {#getLabel--}
```
public final int getLabel()
```


टाइमस्केल टियर के लिए तिथि लेबल [DateLabel](../../com.aspose.tasks/datelabel) प्राप्त करता है।

**Returns:**
int - टाइमस्केल टियर के लिए तिथि लेबल [DateLabel](../../com.aspose.tasks/datelabel).
### getRenderLabelOnEachPage() {#getRenderLabelOnEachPage--}
```
public final boolean getRenderLabelOnEachPage()
```


फ़्लैग प्राप्त करता है जो निर्धारित करता है कि जब एक समय अवधि कई पृष्ठों में फैली हो तो प्रत्येक पृष्ठ पर तिथि लेबल रेंडर किए जाने चाहिए या नहीं। यदि मान 'true' है, तो जब समय अवधि कई पृष्ठों में फैली हो, तो उस अवधि के तिथि लेबल प्रत्येक पृष्ठ पर रेंडर होते हैं। यदि मान 'false' है, तो तिथि लेबल केवल एक बार रेंडर होता है, `Alignment`([getAlignment](../../com.aspose.tasks/timescaletier\#getAlignment--)/[setAlignment(int)](../../com.aspose.tasks/timescaletier\#setAlignment-int-)) प्रॉपर्टी के मान के अनुसार।

--------------------

MS Project में इसका समकक्ष नहीं है।

**Returns:**
बूलियन - वह फ़्लैग जो निर्धारित करता है कि जब कोई समय अवधि कई पृष्ठों में फैली हो तो प्रत्येक पृष्ठ पर तिथि लेबल रेंडर किए जाएँ।
### getShowTicks() {#getShowTicks--}
```
public final boolean getShowTicks()
```


टियर में समय अवधियों को अलग करने वाले टिक मार्क दिखाने के बारे में संकेत देने वाला मान प्राप्त करता है।

**Returns:**
बूलियन - एक मान जो दर्शाता है कि टियर में समय अवधियों को अलग करने वाले टिक मार्क दिखाए जाएँ या नहीं।
### getUnit() {#getUnit--}
```
public final int getUnit()
```


टाइमस्केल टियर के लिए टाइमस्केल यूनिट [TimescaleUnit](../../com.aspose.tasks/timescaleunit) प्राप्त करता है। डिफ़ॉल्ट मान है [TimescaleUnit](../../com.aspose.tasks/timescaleunit)।

**Returns:**
इंट - टाइमस्केल टियर के लिए टाइमस्केल यूनिट [TimescaleUnit](../../com.aspose.tasks/timescaleunit)।
### getUsesFiscalYear() {#getUsesFiscalYear--}
```
public final boolean getUsesFiscalYear()
```


टियर लेबल को वित्तीय वर्ष पर आधारित करने के बारे में संकेत देने वाला मान प्राप्त करता है।

**Returns:**
बूलियन - एक मान जो दर्शाता है कि टियर लेबल को वित्तीय वर्ष पर आधारित किया जाए या नहीं।
### setAlignment(int value) {#setAlignment-int-}
```
public final void setAlignment(int value)
```


टियर के प्रत्येक समय अवधि के भीतर लेबल को कैसे संरेखित किया जाए, सेट करता है ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | int | टियर की प्रत्येक समय अवधि के भीतर लेबल को कैसे संरेखित किया जाए ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |

### setCount(int value) {#setCount-int-}
```
public final void setCount(int value)
```


टियर के लिए लेबल दिखाने वाले समय इकाई अंतराल को सेट करता है। डिफ़ॉल्ट मान 1 है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | टियर के लिए लेबल दिखाने वाला समय इकाई अंतराल। |

### setDateTimeConverter(DateTimeConverter value) {#setDateTimeConverter-com.aspose.tasks.DateTimeConverter-}
```
public final void setDateTimeConverter(DateTimeConverter value)
```


इस टियर में तिथि टिक रेंडरिंग को संभालने के लिए एक कॉलबैक फ़ंक्शन सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [DateTimeConverter](../../com.aspose.tasks/datetimeconverter) | इस टियर में तिथि टिक रेंडरिंग को संभालने के लिए एक कॉलबैक फ़ंक्शन। |

### setLabel(int value) {#setLabel-int-}
```
public final void setLabel(int value)
```


टाइमस्केल टियर के लिए तिथि लेबल [DateLabel](../../com.aspose.tasks/datelabel) सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | int | टाइमस्केल टियर के लिए तिथि लेबल [DateLabel](../../com.aspose.tasks/datelabel)। |

### setRenderLabelOnEachPage(boolean value) {#setRenderLabelOnEachPage-boolean-}
```
public final void setRenderLabelOnEachPage(boolean value)
```


फ़्लैग सेट करता है जो निर्धारित करता है कि जब कोई समय अवधि कई पृष्ठों में फैली हो तो प्रत्येक पृष्ठ पर तिथि लेबल रेंडर किए जाएँ। यदि मान 'true' है, तो जब समय अवधि कई पृष्ठों में फैली हो, अवधि के तिथि लेबल प्रत्येक पृष्ठ पर रेंडर होते हैं। यदि मान 'false' है, तो तिथि लेबल केवल एक बार रेंडर होता है, `Alignment`([getAlignment](../../com.aspose.tasks/timescaletier\#getAlignment--)/[setAlignment(int)](../../com.aspose.tasks/timescaletier\#setAlignment-int-)) प्रॉपर्टी के मान के अनुसार।

--------------------

MS Project में इसका समकक्ष नहीं है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | फ़्लैग जो निर्धारित करता है कि जब कोई समय अवधि कई पृष्ठों में फैली हो तो प्रत्येक पृष्ठ पर तिथि लेबल रेंडर किए जाएँ। |

### setShowTicks(boolean value) {#setShowTicks-boolean-}
```
public final void setShowTicks(boolean value)
```


टियर में समय अवधियों को अलग करने वाले टिक मार्क दिखाने के बारे में संकेत देने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि टियर में समय अवधियों को अलग करने वाले टिक मार्क दिखाए जाएँ या नहीं। |

### setUnit(int value) {#setUnit-int-}
```
public final void setUnit(int value)
```


टाइमस्केल टियर के लिए टाइमस्केल यूनिट [TimescaleUnit](../../com.aspose.tasks/timescaleunit) सेट करता है। डिफ़ॉल्ट मान है [TimescaleUnit](../../com.aspose.tasks/timescaleunit)।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | int | टाइमस्केल टियर के लिए टाइमस्केल यूनिट [TimescaleUnit](../../com.aspose.tasks/timescaleunit)। |

### setUsesFiscalYear(boolean value) {#setUsesFiscalYear-boolean-}
```
public final void setUsesFiscalYear(boolean value)
```


टियर लेबल को वित्तीय वर्ष पर आधारित करने के बारे में संकेत देने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि टियर लेबल को वित्तीय वर्ष पर आधारित किया जाए या नहीं। |

