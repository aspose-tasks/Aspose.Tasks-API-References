---
title: "PixelFormat"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "छवि में प्रत्येक पिक्सेल के रंग डेटा के फ़ॉर्मेट को निर्दिष्ट करता है।"
type: docs
weight: 193
url: /hi/java/com.aspose.tasks/pixelformat/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class PixelFormat extends System.Enum
```

छवि में प्रत्येक पिक्सेल के रंग डेटा के फ़ॉर्मेट को निर्दिष्ट करता है।
## फ़ील्ड्स

| फ़ील्ड | विवरण |
| --- | --- |
| [Alpha](#Alpha) | पिक्सेल डेटा में अल्फा मान होते हैं जो प्री-मल्टिप्लाइड नहीं हैं। |
| [Canonical](#Canonical) | डिफ़ॉल्ट पिक्सेल फ़ॉर्मेट 32 बिट्स प्रति पिक्सेल का है। |
| [DontCare](#DontCare) | कोई पिक्सेल फ़ॉर्मेट निर्दिष्ट नहीं किया गया है। |
| [Extended](#Extended) | आरक्षित। |
| [Format16bppArgb1555](#Format16bppArgb1555) | पिक्सेल फ़ॉर्मेट 16 बिट प्रति पिक्सेल है। |
| [Format16bppGrayScale](#Format16bppGrayScale) | पिक्सेल फ़ॉर्मेट 16 बिट प्रति पिक्सेल है। |
| [Format16bppRgb555](#Format16bppRgb555) | निर्दिष्ट करता है कि फ़ॉर्मेट 16 बिट प्रति पिक्सेल है; प्रत्येक लाल, हरे और नीले घटकों के लिए 5 बिट उपयोग किए जाते हैं। |
| [Format16bppRgb565](#Format16bppRgb565) | निर्दिष्ट करता है कि फ़ॉर्मेट 16 बिट प्रति पिक्सेल है; लाल घटक के लिए 5 बिट, हरे घटक के लिए 6 बिट, और नीले घटक के लिए 5 बिट उपयोग किए जाते हैं। |
| [Format1bppIndexed](#Format1bppIndexed) | निर्दिष्ट करता है कि पिक्सेल फ़ॉर्मेट 1 बिट प्रति पिक्सेल है और यह अनुक्रमित रंग का उपयोग करता है। |
| [Format24bppRgb](#Format24bppRgb) | निर्दिष्ट करता है कि फ़ॉर्मेट 24 बिट प्रति पिक्सेल है; प्रत्येक लाल, हरे और नीले घटकों के लिए 8 बिट उपयोग किए जाते हैं। |
| [Format32bppArgb](#Format32bppArgb) | निर्दिष्ट करता है कि फ़ॉर्मेट 32 बिट प्रति पिक्सेल है; अल्फा, लाल, हरे और नीले घटकों के लिए प्रत्येक 8 बिट उपयोग किए जाते हैं। |
| [Format32bppPArgb](#Format32bppPArgb) | निर्दिष्ट करता है कि फ़ॉर्मेट 32 बिट प्रति पिक्सेल है; अल्फा, लाल, हरे और नीले घटकों के लिए प्रत्येक 8 बिट उपयोग किए जाते हैं। |
| [Format32bppRgb](#Format32bppRgb) | निर्दिष्ट करता है कि फ़ॉर्मेट 32 बिट प्रति पिक्सेल है; प्रत्येक लाल, हरे और नीले घटकों के लिए 8 बिट उपयोग किए जाते हैं। |
| [Format48bppRgb](#Format48bppRgb) | निर्दिष्ट करता है कि फ़ॉर्मेट 48 बिट प्रति पिक्सेल है; प्रत्येक लाल, हरे और नीले घटकों के लिए 16 बिट उपयोग किए जाते हैं। |
| [Format4bppIndexed](#Format4bppIndexed) | निर्दिष्ट करता है कि फ़ॉर्मेट 4 बिट प्रति पिक्सेल है, अनुक्रमित। |
| [Format64bppArgb](#Format64bppArgb) | निर्दिष्ट करता है कि फ़ॉर्मेट 64 बिट प्रति पिक्सेल है; अल्फा, लाल, हरे और नीले घटकों के लिए प्रत्येक 16 बिट उपयोग किए जाते हैं। |
| [Format64bppPArgb](#Format64bppPArgb) | निर्दिष्ट करता है कि फ़ॉर्मेट 64 बिट प्रति पिक्सेल है; अल्फा, लाल, हरे और नीले घटकों के लिए प्रत्येक 16 बिट उपयोग किए जाते हैं। |
| [Format8bppIndexed](#Format8bppIndexed) | निर्दिष्ट करता है कि फ़ॉर्मेट 8 बिट प्रति पिक्सेल है, अनुक्रमित। |
| [Gdi](#Gdi) | पिक्सेल डेटा में GDI रंग शामिल हैं। |
| [Indexed](#Indexed) | पिक्सेल डेटा में रंग-इंडेक्स्ड मान शामिल हैं, जिसका अर्थ है कि मान सिस्टम रंग तालिका में रंगों के लिए एक इंडेक्स हैं, व्यक्तिगत रंग मानों के बजाय। |
| [Max](#Max) | इस एनीमरेशन के लिए अधिकतम मान। |
| [PAlpha](#PAlpha) | पिक्सेल फ़ॉर्मेट में प्रीमल्टिप्लाइड अल्फा मान शामिल हैं। |
| [Undefined](#Undefined) | पिक्सेल फ़ॉर्मेट अपरिभाषित है। |
### Alpha {#Alpha}
```
public static final int Alpha
```


पिक्सेल डेटा में अल्फा मान होते हैं जो प्री-मल्टिप्लाइड नहीं हैं।

### Canonical {#Canonical}
```
public static final int Canonical
```


डिफ़ॉल्ट पिक्सेल फ़ॉर्मेट 32 बिट प्रति पिक्सेल है। फ़ॉर्मेट 24-बिट रंग गहराई और 8-बिट अल्फा चैनल निर्दिष्ट करता है।

### DontCare {#DontCare}
```
public static final int DontCare
```


कोई पिक्सेल फ़ॉर्मेट निर्दिष्ट नहीं किया गया है।

### Extended {#Extended}
```
public static final int Extended
```


आरक्षित।

### Format16bppArgb1555 {#Format16bppArgb1555}
```
public static final int Format16bppArgb1555
```


पिक्सेल फ़ॉर्मेट 16 बिट प्रति पिक्सेल है। रंग जानकारी 32,768 रंग शेड्स निर्दिष्ट करती है, जिसमें 5 बिट लाल, 5 बिट हरा, 5 बिट नीला और 1 बिट अल्फा है।

### Format16bppGrayScale {#Format16bppGrayScale}
```
public static final int Format16bppGrayScale
```


पिक्सेल फ़ॉर्मेट 16 बिट प्रति पिक्सेल है। रंग जानकारी 65,536 ग्रे शेड्स निर्दिष्ट करती है।

### Format16bppRgb555 {#Format16bppRgb555}
```
public static final int Format16bppRgb555
```


निर्दिष्ट करता है कि फ़ॉर्मेट 16 बिट प्रति पिक्सेल है; प्रत्येक लाल, हरे और नीले घटकों के लिए 5 बिट उपयोग किए जाते हैं। शेष बिट उपयोग नहीं किया जाता।

### Format16bppRgb565 {#Format16bppRgb565}
```
public static final int Format16bppRgb565
```


निर्दिष्ट करता है कि फ़ॉर्मेट 16 बिट प्रति पिक्सेल है; लाल घटक के लिए 5 बिट, हरे घटक के लिए 6 बिट, और नीले घटक के लिए 5 बिट उपयोग किए जाते हैं।

### Format1bppIndexed {#Format1bppIndexed}
```
public static final int Format1bppIndexed
```


निर्दिष्ट करता है कि पिक्सेल फ़ॉर्मेट 1 बिट प्रति पिक्सेल है और यह अनुक्रमित रंग का उपयोग करता है। इसलिए रंग तालिका में दो रंग होते हैं।

### Format24bppRgb {#Format24bppRgb}
```
public static final int Format24bppRgb
```


निर्दिष्ट करता है कि फ़ॉर्मेट 24 बिट प्रति पिक्सेल है; प्रत्येक लाल, हरे और नीले घटकों के लिए 8 बिट उपयोग किए जाते हैं।

### Format32bppArgb {#Format32bppArgb}
```
public static final int Format32bppArgb
```


निर्दिष्ट करता है कि फ़ॉर्मेट 32 बिट प्रति पिक्सेल है; अल्फा, लाल, हरे और नीले घटकों के लिए प्रत्येक 8 बिट उपयोग किए जाते हैं।

### Format32bppPArgb {#Format32bppPArgb}
```
public static final int Format32bppPArgb
```


निर्दिष्ट करता है कि फ़ॉर्मेट 32 बिट प्रति पिक्सेल है; अल्फा, लाल, हरे और नीले घटकों के लिए प्रत्येक 8 बिट उपयोग किए जाते हैं। अल्फा घटक के अनुसार लाल, हरे और नीले घटकों को प्रीमल्टिप्लाइड किया गया है।

### Format32bppRgb {#Format32bppRgb}
```
public static final int Format32bppRgb
```


निर्दिष्ट करता है कि फ़ॉर्मेट 32 बिट प्रति पिक्सेल है; प्रत्येक लाल, हरे और नीले घटकों के लिए 8 बिट उपयोग किए जाते हैं। शेष 8 बिट उपयोग नहीं किए जाते।

### Format48bppRgb {#Format48bppRgb}
```
public static final int Format48bppRgb
```


निर्दिष्ट करता है कि फ़ॉर्मेट 48 बिट प्रति पिक्सेल है; प्रत्येक लाल, हरे और नीले घटकों के लिए 16 बिट उपयोग किए जाते हैं।

### Format4bppIndexed {#Format4bppIndexed}
```
public static final int Format4bppIndexed
```


निर्दिष्ट करता है कि फ़ॉर्मेट 4 बिट प्रति पिक्सेल है, अनुक्रमित।

### Format64bppArgb {#Format64bppArgb}
```
public static final int Format64bppArgb
```


निर्दिष्ट करता है कि फ़ॉर्मेट 64 बिट प्रति पिक्सेल है; अल्फा, लाल, हरे और नीले घटकों के लिए प्रत्येक 16 बिट उपयोग किए जाते हैं।

### Format64bppPArgb {#Format64bppPArgb}
```
public static final int Format64bppPArgb
```


निर्दिष्ट करता है कि फ़ॉर्मेट 64 बिट प्रति पिक्सेल है; प्रत्येक 16 बिट अल्फा, लाल, हरा और नीले घटकों के लिए उपयोग होते हैं। लाल, हरे और नीले घटकों को अल्फा घटक के अनुसार प्री‑मल्टिप्लाई किया जाता है।

### Format8bppIndexed {#Format8bppIndexed}
```
public static final int Format8bppIndexed
```


निर्दिष्ट करता है कि फ़ॉर्मेट 8 बिट प्रति पिक्सेल है, अनुक्रमित। इसलिए रंग तालिका में 256 रंग होते हैं।

### Gdi {#Gdi}
```
public static final int Gdi
```


पिक्सेल डेटा में GDI रंग शामिल हैं।

### Indexed {#Indexed}
```
public static final int Indexed
```


पिक्सेल डेटा में रंग-इंडेक्स्ड मान शामिल हैं, जिसका अर्थ है कि मान सिस्टम रंग तालिका में रंगों के लिए एक इंडेक्स हैं, व्यक्तिगत रंग मानों के बजाय।

### Max {#Max}
```
public static final int Max
```


इस एनीमरेशन के लिए अधिकतम मान।

### PAlpha {#PAlpha}
```
public static final int PAlpha
```


पिक्सेल फ़ॉर्मेट में प्रीमल्टिप्लाइड अल्फा मान शामिल हैं।

### Undefined {#Undefined}
```
public static final int Undefined
```


पिक्सेल फ़ॉर्मेट अपरिभाषित है।

