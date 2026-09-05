---
title: "UsageView"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "प्रोजेक्ट में एक उपयोग दृश्य को दर्शाता है।"
type: docs
weight: 331
url: /hi/java/com.aspose.tasks/usageview/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.View](../../com.aspose.tasks/view)

**All Implemented Interfaces:**
com.aspose.tasks.ITimescaledView
```
public abstract class UsageView extends View implements ITimescaledView
```

प्रोजेक्ट में एक उपयोग दृश्य को दर्शाता है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getAlignDetailsData()](#getAlignDetailsData--) | विवरण डेटा संरेखण प्राप्त करता है। |
| [getBottomTimescaleTier()](#getBottomTimescaleTier--) | व्यू के नीचे के टाइमस्केल टियर की सेटिंग्स प्राप्त करता है। |
| [getDisplayDetailsHeaderColumn()](#getDisplayDetailsHeaderColumn--) | व्यू में विवरण हेडर कॉलम प्रदर्शित करने के लिए है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getDisplayShortDetailHeaderNames()](#getDisplayShortDetailHeaderNames--) | छोटे विवरण हेडर नाम प्रदर्शित करने के लिए है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getMiddleTimescaleTier()](#getMiddleTimescaleTier--) | व्यू के मध्य टाइमस्केल टियर की सेटिंग्स प्राप्त करता है। |
| [getRepeatDetailsHeaderOnAllRows()](#getRepeatDetailsHeaderOnAllRows--) | सभी असाइनमेंट पंक्तियों पर विवरण हेडर दोहराने के लिए है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getTimescaleSizePercentage()](#getTimescaleSizePercentage--) | \{@inheritDoc\} |
| [getTopTimescaleTier()](#getTopTimescaleTier--) | व्यू के शीर्ष टाइमस्केल टियर की सेटिंग्स प्राप्त करता है। |
| [setAlignDetailsData(int value)](#setAlignDetailsData-int-) | विवरण डेटा संरेखण सेट करता है। |
| [setBottomTimescaleTier(TimescaleTier value)](#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-) | व्यू के नीचे के टाइमस्केल टियर की सेटिंग्स सेट करता है। |
| [setDisplayDetailsHeaderColumn(boolean value)](#setDisplayDetailsHeaderColumn-boolean-) | व्यू में विवरण हेडर कॉलम प्रदर्शित करने के लिए है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setDisplayShortDetailHeaderNames(boolean value)](#setDisplayShortDetailHeaderNames-boolean-) | छोटे विवरण हेडर नाम प्रदर्शित करने के लिए है या नहीं, यह दर्शाने वाला मान सेट करता है। |
| [setMiddleTimescaleTier(TimescaleTier value)](#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-) | दृश्य की मध्य टाइमस्केल टियर की सेटिंग्स सेट करता है। |
| [setRepeatDetailsHeaderOnAllRows(boolean value)](#setRepeatDetailsHeaderOnAllRows-boolean-) | एक मान सेट करता है जो दर्शाता है कि सभी असाइनमेंट पंक्तियों में विवरण हेडर दोहराया जाए या नहीं। |
| [setTimescaleSizePercentage(int value)](#setTimescaleSizePercentage-int-) | \{@inheritDoc\} |
| [setTopTimescaleTier(TimescaleTier value)](#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-) | दृश्य की शीर्ष टाइमस्केल टियर की सेटिंग्स सेट करता है। |
### getAlignDetailsData() {#getAlignDetailsData--}
```
public final int getAlignDetailsData()
```


विवरण डेटा संरेखण प्राप्त करता है।

**Returns:**
int - विवरण डेटा संरेखण।
### getBottomTimescaleTier() {#getBottomTimescaleTier--}
```
public final TimescaleTier getBottomTimescaleTier()
```


दृश्य की निचली टाइमस्केल टियर की सेटिंग्स प्राप्त करता है। [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's bottom timescale tier.
### getDisplayDetailsHeaderColumn() {#getDisplayDetailsHeaderColumn--}
```
public final boolean getDisplayDetailsHeaderColumn()
```


व्यू में विवरण हेडर कॉलम प्रदर्शित करने के लिए है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
boolean - एक मान जो दर्शाता है कि दृश्य में विवरण हेडर कॉलम प्रदर्शित किया जाए या नहीं।
### getDisplayShortDetailHeaderNames() {#getDisplayShortDetailHeaderNames--}
```
public final boolean getDisplayShortDetailHeaderNames()
```


छोटे विवरण हेडर नाम प्रदर्शित करने के लिए है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
boolean - एक मान जो दर्शाता है कि संक्षिप्त विवरण हेडर नाम प्रदर्शित किए जाएँ या नहीं।
### getMiddleTimescaleTier() {#getMiddleTimescaleTier--}
```
public final TimescaleTier getMiddleTimescaleTier()
```


दृश्य की मध्य टाइमस्केल टियर की सेटिंग्स प्राप्त करता है। [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's middle timescale tier.
### getRepeatDetailsHeaderOnAllRows() {#getRepeatDetailsHeaderOnAllRows--}
```
public final boolean getRepeatDetailsHeaderOnAllRows()
```


सभी असाइनमेंट पंक्तियों पर विवरण हेडर दोहराने के लिए है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
boolean - एक मान जो दर्शाता है कि सभी असाइनमेंट पंक्तियों में विवरण हेडर दोहराया जाए या नहीं।
### getTimescaleSizePercentage() {#getTimescaleSizePercentage--}
```
public final int getTimescaleSizePercentage()
```


टाइमस्केल टियर पर इकाइयों के बीच की दूरी को घटाने या बढ़ाने के लिए प्रतिशत प्राप्त करता है।

**Returns:**
int - \{@inheritDoc\}
### getTopTimescaleTier() {#getTopTimescaleTier--}
```
public final TimescaleTier getTopTimescaleTier()
```


दृश्य की शीर्ष टाइमस्केल टियर की सेटिंग्स प्राप्त करता है। [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's top timescale tier.
### setAlignDetailsData(int value) {#setAlignDetailsData-int-}
```
public final void setAlignDetailsData(int value)
```


विवरण डेटा संरेखण सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | विवरण डेटा संरेखण। |

### setBottomTimescaleTier(TimescaleTier value) {#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setBottomTimescaleTier(TimescaleTier value)
```


दृश्य की निचली टाइमस्केल टियर की सेटिंग्स सेट करता है। [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | दृश्य की निचली टाइमस्केल टियर की सेटिंग्स। |

### setDisplayDetailsHeaderColumn(boolean value) {#setDisplayDetailsHeaderColumn-boolean-}
```
public final void setDisplayDetailsHeaderColumn(boolean value)
```


व्यू में विवरण हेडर कॉलम प्रदर्शित करने के लिए है या नहीं, यह दर्शाने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि दृश्य में विवरण हेडर कॉलम प्रदर्शित किया जाए या नहीं। |

### setDisplayShortDetailHeaderNames(boolean value) {#setDisplayShortDetailHeaderNames-boolean-}
```
public final void setDisplayShortDetailHeaderNames(boolean value)
```


छोटे विवरण हेडर नाम प्रदर्शित करने के लिए है या नहीं, यह दर्शाने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि संक्षिप्त विवरण हेडर नाम प्रदर्शित किए जाएँ या नहीं। |

### setMiddleTimescaleTier(TimescaleTier value) {#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setMiddleTimescaleTier(TimescaleTier value)
```


दृश्य की मध्य टाइमस्केल टियर की सेटिंग्स सेट करता है। [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | दृश्य की मध्य टाइमस्केल टियर की सेटिंग्स। |

### setRepeatDetailsHeaderOnAllRows(boolean value) {#setRepeatDetailsHeaderOnAllRows-boolean-}
```
public final void setRepeatDetailsHeaderOnAllRows(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि सभी असाइनमेंट पंक्तियों में विवरण हेडर दोहराया जाए या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | boolean | एक मान जो दर्शाता है कि सभी असाइनमेंट पंक्तियों में विवरण हेडर दोहराया जाए या नहीं। |

### setTimescaleSizePercentage(int value) {#setTimescaleSizePercentage-int-}
```
public final void setTimescaleSizePercentage(int value)
```


टाइमस्केल टियर पर इकाइयों के बीच की दूरी को घटाने या बढ़ाने के लिए प्रतिशत सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | \{@inheritDoc\} |

### setTopTimescaleTier(TimescaleTier value) {#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setTopTimescaleTier(TimescaleTier value)
```


दृश्य की शीर्ष टाइमस्केल टियर की सेटिंग्स सेट करता है। [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | दृश्य की शीर्ष टाइमस्केल टियर की सेटिंग्स। |

