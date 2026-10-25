---
title: "दर"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "उस अवधि के दौरान संसाधन पर लागू समय अवधि और दरों की परिभाषा का प्रतिनिधित्व करता है।"
type: docs
weight: 232
url: /hi/java/com.aspose.tasks/rate/
---

**Inheritance:**
java.lang.Object
```
public class Rate
```

उस अवधि के दौरान संसाधन पर लागू समय अवधि और दरों की परिभाषा का प्रतिनिधित्व करता है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [getCostPerUse()](#getCostPerUse--) | एक resource के प्रति उपयोग लागत प्राप्त करता है। |
| [getOvertimeRate()](#getOvertimeRate--) | एक resource के लिए प्रति घंटे overtime दर प्राप्त करता है। |
| [getOvertimeRateFormat()](#getOvertimeRateFormat--) | Microsoft Project द्वारा overtime दर दिखाने के लिए उपयोग किए गए इकाइयों को प्राप्त करता है। |
| [getRateTable()](#getRateTable--) | एक resource के लिए rate table का अनूठा पहचानकर्ता प्राप्त करता है। |
| [getRatesFrom()](#getRatesFrom--) | जब एक दर प्रभावी होती है, उस तिथि को प्राप्त करता है। |
| [getRatesTo()](#getRatesTo--) | जब एक दर प्रभावी होती है, अंतिम तिथि को प्राप्त करता है। |
| [getStandardRate()](#getStandardRate--) | एक resource के लिए प्रति घंटे मानक दर प्राप्त करता है। |
| [getStandardRateFormat()](#getStandardRateFormat--) | Microsoft Project द्वारा मानक दर दिखाने के लिए उपयोग किए गए इकाइयों को प्राप्त करता है। |
| [setCostPerUse(BigDecimal value)](#setCostPerUse-java.math.BigDecimal-) | संसाधन के प्रति उपयोग लागत सेट करता है। |
| [setOvertimeRate(BigDecimal value)](#setOvertimeRate-java.math.BigDecimal-) | संसाधन के लिए प्रति घंटे ओवरटाइम दर सेट करता है। |
| [setOvertimeRateFormat(int value)](#setOvertimeRateFormat-int-) | Microsoft Project द्वारा ओवरटाइम दर दिखाने के लिए उपयोग किए जाने वाले इकाइयों को सेट करता है। |
| [setRateTable(int value)](#setRateTable-int-) | संसाधन के लिए दर तालिका का अनूठा पहचानकर्ता सेट करता है। |
| [setRatesFrom(Date value)](#setRatesFrom-java.util.Date-) | दर के प्रभावी होने की तिथि सेट करता है। |
| [setRatesTo(Date value)](#setRatesTo-java.util.Date-) | दर के प्रभावी रहने की अंतिम तिथि सेट करता है। |
| [setStandardRate(BigDecimal value)](#setStandardRate-java.math.BigDecimal-) | संसाधन के लिए प्रति घंटे मानक दर सेट करता है। |
| [setStandardRateFormat(int value)](#setStandardRateFormat-int-) | Microsoft Project द्वारा मानक दर दिखाने के लिए उपयोग किए जाने वाले इकाइयों को सेट करता है। |
### getCostPerUse() {#getCostPerUse--}
```
public final BigDecimal getCostPerUse()
```


संसाधन के प्रति उपयोग लागत प्राप्त करता है। यह मान वर्तमान तिथि से प्राप्त किया जाता है यदि संसाधन के लिए दर तालिका मौजूद है।

**Returns:**
java.math.BigDecimal - संसाधन के प्रति उपयोग लागत।
### getOvertimeRate() {#getOvertimeRate--}
```
public final BigDecimal getOvertimeRate()
```


एक resource के लिए प्रति घंटे overtime दर प्राप्त करता है।

**Returns:**
java.math.BigDecimal - संसाधन के लिए प्रति घंटे ओवरटाइम दर।
### getOvertimeRateFormat() {#getOvertimeRateFormat--}
```
public final int getOvertimeRateFormat()
```


Microsoft Project द्वारा overtime दर दिखाने के लिए उपयोग किए गए इकाइयों को प्राप्त करता है।

**Returns:**
int - Microsoft Project द्वारा ओवरटाइम दर दिखाने के लिए उपयोग की जाने वाली इकाइयाँ।
### getRateTable() {#getRateTable--}
```
public final int getRateTable()
```


एक resource के लिए rate table का अनूठा पहचानकर्ता प्राप्त करता है।

**Returns:**
int - संसाधन के लिए दर तालिका का अनूठा पहचानकर्ता।
### getRatesFrom() {#getRatesFrom--}
```
public final Date getRatesFrom()
```


जब एक दर प्रभावी होती है, उस तिथि को प्राप्त करता है।

**Returns:**
java.util.Date - दर के प्रभावी होने की तिथि।
### getRatesTo() {#getRatesTo--}
```
public final Date getRatesTo()
```


जब एक दर प्रभावी होती है, अंतिम तिथि को प्राप्त करता है।

**Returns:**
java.util.Date - दर के प्रभावी रहने की अंतिम तिथि।
### getStandardRate() {#getStandardRate--}
```
public final BigDecimal getStandardRate()
```


एक resource के लिए प्रति घंटे मानक दर प्राप्त करता है।

**Returns:**
java.math.BigDecimal - संसाधन के लिए प्रति घंटे मानक दर।
### getStandardRateFormat() {#getStandardRateFormat--}
```
public final int getStandardRateFormat()
```


Microsoft Project द्वारा मानक दर दिखाने के लिए उपयोग किए गए इकाइयों को प्राप्त करता है।

**Returns:**
int - Microsoft Project द्वारा मानक दर दिखाने के लिए उपयोग की जाने वाली इकाइयाँ।
### setCostPerUse(BigDecimal value) {#setCostPerUse-java.math.BigDecimal-}
```
public final void setCostPerUse(BigDecimal value)
```


संसाधन के प्रति उपयोग लागत सेट करता है। यह मान वर्तमान तिथि से प्राप्त किया जाता है यदि संसाधन के लिए दर तालिका मौजूद है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.math.BigDecimal | संसाधन के प्रति उपयोग लागत। |

### setOvertimeRate(BigDecimal value) {#setOvertimeRate-java.math.BigDecimal-}
```
public final void setOvertimeRate(BigDecimal value)
```


संसाधन के लिए प्रति घंटे ओवरटाइम दर सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.math.BigDecimal | संसाधन के लिए प्रति घंटे ओवरटाइम दर। |

### setOvertimeRateFormat(int value) {#setOvertimeRateFormat-int-}
```
public final void setOvertimeRateFormat(int value)
```


Microsoft Project द्वारा ओवरटाइम दर दिखाने के लिए उपयोग किए जाने वाले इकाइयों को सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | Microsoft Project द्वारा ओवरटाइम दर दिखाने के लिए उपयोग की जाने वाली इकाइयाँ। |

### setRateTable(int value) {#setRateTable-int-}
```
public final void setRateTable(int value)
```


संसाधन के लिए दर तालिका का अनूठा पहचानकर्ता सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | संसाधन के लिए दर तालिका का अनूठा पहचानकर्ता। |

### setRatesFrom(Date value) {#setRatesFrom-java.util.Date-}
```
public final void setRatesFrom(Date value)
```


दर के प्रभावी होने की तिथि सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | दर के प्रभावी होने की तिथि। |

### setRatesTo(Date value) {#setRatesTo-java.util.Date-}
```
public final void setRatesTo(Date value)
```


दर के प्रभावी रहने की अंतिम तिथि सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | दर के प्रभावी रहने की अंतिम तिथि। |

### setStandardRate(BigDecimal value) {#setStandardRate-java.math.BigDecimal-}
```
public final void setStandardRate(BigDecimal value)
```


संसाधन के लिए प्रति घंटे मानक दर सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.math.BigDecimal | संसाधन के लिए प्रति घंटे मानक दर। |

### setStandardRateFormat(int value) {#setStandardRateFormat-int-}
```
public final void setStandardRateFormat(int value)
```


Microsoft Project द्वारा मानक दर दिखाने के लिए उपयोग किए जाने वाले इकाइयों को सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | Microsoft Project द्वारा मानक दर प्रदर्शित करने के लिए उपयोग की जाने वाली इकाइयाँ। |

