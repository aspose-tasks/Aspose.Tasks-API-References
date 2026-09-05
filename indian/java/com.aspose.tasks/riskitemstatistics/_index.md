---
title: "RiskItemStatistics"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "एक आइटम का प्रतिनिधित्व करता है जो विश्लेषित परियोजना के कार्य के लिए सांख्यिकीय डेटा संग्रहीत करता है।"
type: docs
weight: 265
url: /hi/java/com.aspose.tasks/riskitemstatistics/
---

**Inheritance:**
java.lang.Object
```
public class RiskItemStatistics
```

एक आइटम का प्रतिनिधित्व करता है जो विश्लेषित परियोजना के कार्य के लिए सांख्यिकीय डेटा संग्रहीत करता है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getExpectedValue()](#getExpectedValue--) | रिस्क आइटम का अपेक्षित मान प्राप्त करता है। |
| [getItemType()](#getItemType--) | [RiskItemType](../../com.aspose.tasks/riskitemtype) enumeration का एक इंस्टेंस प्राप्त करता है। |
| [getMaximum()](#getMaximum--) | Monte Carlo सिमुलेशन के दौरान उत्पन्न अधिकतम मान प्राप्त करता है। |
| [getMinimum()](#getMinimum--) | Monte Carlo सिमुलेशन के दौरान उत्पन्न न्यूनतम मान प्राप्त करता है। |
| [getPercentile(int percent)](#getPercentile-int-) | एक मान प्राप्त करता है जिसके नीचे उत्पन्न नमूनों का निर्दिष्ट प्रतिशत गिरता है। |
| [getStandardDeviation()](#getStandardDeviation--) | रिस्क आइटम का मानक विचलन प्राप्त करता है। |
| [toString()](#toString--) | रिस्क आइटम का संक्षिप्त स्ट्रिंग प्रतिनिधित्व लौटाता है। |
### getExpectedValue() {#getExpectedValue--}
```
public final Date getExpectedValue()
```


रिस्क आइटम का अपेक्षित मान प्राप्त करता है।

**Returns:**
java.util.Date - जोखिम आइटम का अपेक्षित मान।
### getItemType() {#getItemType--}
```
public final int getItemType()
```


[RiskItemType](../../com.aspose.tasks/riskitemtype) enumeration का एक इंस्टेंस प्राप्त करता है।

**Returns:**
int - [RiskItemType](../../com.aspose.tasks/riskitemtype) एन्यूमरेशन का एक उदाहरण।
### getMaximum() {#getMaximum--}
```
public final Date getMaximum()
```


Monte Carlo सिमुलेशन के दौरान उत्पन्न अधिकतम मान प्राप्त करता है।

**Returns:**
java.util.Date - मोन्टे कार्लो सिमुलेशन के दौरान उत्पन्न अधिकतम मान।
### getMinimum() {#getMinimum--}
```
public final Date getMinimum()
```


Monte Carlo सिमुलेशन के दौरान उत्पन्न न्यूनतम मान प्राप्त करता है।

**Returns:**
java.util.Date - मोन्टे कार्लो सिमुलेशन के दौरान उत्पन्न न्यूनतम मान।
### getPercentile(int percent) {#getPercentile-int-}
```
public final Date getPercentile(int percent)
```


एक मान प्राप्त करता है जिसके नीचे उत्पन्न नमूनों का निर्दिष्ट प्रतिशत गिरता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रतिशत | int | 0 और 100 के बीच निर्दिष्ट प्रतिशत। |

**Returns:**
java.util.Date - एक मान जिसके नीचे उत्पन्न नमूनों का निर्दिष्ट प्रतिशत गिरता है।
### getStandardDeviation() {#getStandardDeviation--}
```
public final Duration getStandardDeviation()
```


रिस्क आइटम का मानक विचलन प्राप्त करता है।

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the standard deviation of the risk item.
### toString() {#toString--}
```
public String toString()
```


जोखिम आइटम का संक्षिप्त स्ट्रिंग प्रतिनिधित्व लौटाता है। प्रतिनिधित्व के सटीक विवरण अनिर्दिष्ट हैं और परिवर्तन के अधीन हो सकते हैं।

**Returns:**
java.lang.String - RiskItem ऑब्जेक्ट का प्रतिनिधित्व करने वाली संक्षिप्त स्ट्रिंग।
