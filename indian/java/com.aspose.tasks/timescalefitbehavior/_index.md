---
title: "TimescaleFitBehavior"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "पेज की चौड़ाई के साथ टाइमस्केल क्षेत्र को संरेखित करने के लिए उपयोग किए जाने वाले व्यवहार का प्रतिनिधित्व करता है।"
type: docs
weight: 324
url: /hi/java/com.aspose.tasks/timescalefitbehavior/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class TimescaleFitBehavior extends System.Enum
```

पेज की चौड़ाई के साथ टाइमस्केल क्षेत्र को संरेखित करने के लिए उपयोग किए जाने वाले व्यवहार का प्रतिनिधित्व करता है।
## फ़ील्ड्स

| फ़ील्ड | विवरण |
| --- | --- |
| [DefinedInView](#DefinedInView) | कैलेंडर सेक्शन को रेंडर किए गए View की View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage प्रॉपर्टी के अनुसार रेंडर किया जाता है। |
| [NoScaleToEndDate](#NoScaleToEndDate) | कैलेंडर सेक्शन को EndDate तक ठीक-ठीक रेंडर किया जाता है, भले ही पृष्ठ पर खाली स्थान हो। |
| [NoScaleToEndOfPage](#NoScaleToEndOfPage) | कैलेंडर सेक्शन को अंतिम पृष्ठ के अंत (दाएँ पक्ष) तक रेंडर किया जाता है। |
| [ScaleToEndOfPage](#ScaleToEndOfPage) | रेंडरिंग इंजन तिथियों को इस तरह संरेखित करने की कोशिश करेगा कि EndDate अंतिम पृष्ठ के अंत (दाएँ पक्ष) के साथ संरेखित हो। |
### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


कैलेंडर सेक्शन को रेंडर किए गए View की View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage प्रॉपर्टी के अनुसार रेंडर किया जाता है।

### NoScaleToEndDate {#NoScaleToEndDate}
```
public static final int NoScaleToEndDate
```


कैलेंडर सेक्शन को EndDate तक ठीक-ठीक रेंडर किया जाता है, भले ही पृष्ठ पर खाली स्थान हो।

### NoScaleToEndOfPage {#NoScaleToEndOfPage}
```
public static final int NoScaleToEndOfPage
```


कैलेंडर सेक्शन को अंतिम पृष्ठ के अंत (दाएँ पक्ष) तक रेंडर किया जाता है। इसलिए अंतिम रेंडर की गई तिथि EndDate से अधिक हो सकती है।

### ScaleToEndOfPage {#ScaleToEndOfPage}
```
public static final int ScaleToEndOfPage
```


रेंडरिंग इंजन तिथियों को इस तरह संरेखित करने की कोशिश करेगा कि EndDate अंतिम पृष्ठ के अंत (दाएँ पक्ष) के साथ संरेखित हो। यह MS Project के \"Page Setup \\ View \\ Fit timescale to end of page\" विकल्प के सक्षम होने के अनुरूप है।

