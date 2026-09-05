---
title: "बेसलाइन"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "एक संसाधन के बेसलाइन मानों का प्रतिनिधित्व करता है।"
type: docs
weight: 26
url: /hi/java/com.aspose.tasks/baseline/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable, com.aspose.ms.System.IEquatable
```
public class Baseline implements Comparable<Baseline>, System.IEquatable<Baseline>
```

एक संसाधन के बेसलाइन मानों का प्रतिनिधित्व करता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [Baseline()](#Baseline--) |  |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [compareTo(Baseline other)](#compareTo-com.aspose.tasks.Baseline-) | IComparable इंटरफ़ेस कार्यान्वयन। |
| [equals(Baseline other)](#equals-com.aspose.tasks.Baseline-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| [equals(Object obj)](#equals-java.lang.Object-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| [getBaselineNumber()](#getBaselineNumber--) | बेसलाइन डेटा रिकॉर्ड की अद्वितीय संख्या प्राप्त करता है। |
| [getBcwp()](#getBcwp--) | किसी संसाधन द्वारा किसी परियोजना के लिए अब तक किए गए कार्य की बजटेड लागत प्राप्त करता है। |
| [getBcws()](#getBcws--) | संसाधन के लिए निर्धारित कार्य की बजट लागत प्राप्त करता है। |
| [getCost()](#getCost--) | जब बेसलाइन सहेजी जाती है, तब संसाधन की अनुमानित लागत प्राप्त करता है। |
| [getWork()](#getWork--) | जब बेसलाइन सहेजी जाती है, तब संसाधन को सौंपे गए कार्य को प्राप्त करता है। |
| [hashCode()](#hashCode--) | बेसलाइन के लिए हैश कोड मान लौटाता है। |
| [op_Equality(Baseline a, Baseline b)](#op-Equality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| [op_GreaterThan(Baseline a, Baseline b)](#op-GreaterThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से बड़ा है या नहीं। |
| [op_GreaterThanOrEqual(Baseline a, Baseline b)](#op-GreaterThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से बड़ा या बराबर है या नहीं। |
| [op_Inequality(Baseline a, Baseline b)](#op-Inequality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर नहीं है या नहीं। |
| [op_LessThan(Baseline a, Baseline b)](#op-LessThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से छोटा है या नहीं। |
| [op_LessThanOrEqual(Baseline a, Baseline b)](#op-LessThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से छोटा या बराबर है या नहीं। |
| [setBaselineNumber(int value)](#setBaselineNumber-int-) | बेसलाइन डेटा रिकॉर्ड की विशिष्ट संख्या सेट करता है। |
| [setBcwp(double value)](#setBcwp-double-) | किसी संसाधन द्वारा किसी परियोजना के लिए अब तक किए गए कार्य की बजटेड लागत सेट करता है। |
| [setBcws(double value)](#setBcws-double-) | संसाधन के लिए निर्धारित कार्य की बजट लागत सेट करता है। |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | जब बेसलाइन सहेजी जाती है, तब संसाधन की अनुमानित लागत सेट करता है। |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | जब बेसलाइन सहेजी जाती है, तब संसाधन को सौंपे गए कार्य को सेट करता है। |
### Baseline() {#Baseline--}
```
public Baseline()
```


### compareTo(Baseline other) {#compareTo-com.aspose.tasks.Baseline-}
```
public final int compareTo(Baseline other)
```


IComparable इंटरफ़ेस कार्यान्वयन। इस इंस्टेंस की निर्दिष्ट Baseline ऑब्जेक्ट से तुलना करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| other | [Baseline](../../com.aspose.tasks/baseline) | इस इंस्टेंस की तुलना करने के लिए निर्दिष्ट Baseline ऑब्जेक्ट। |

**Returns:**
int - यदि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से कम है तो -1 लौटाता है, यदि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से बड़ा है तो 1; अन्यथा 0 लौटाता है।
### equals(Baseline other) {#equals-com.aspose.tasks.Baseline-}
```
public final boolean equals(Baseline other)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| other | [Baseline](../../com.aspose.tasks/baseline) | इस इंस्टेंस से तुलना करने के लिए निर्दिष्ट ऑब्जेक्ट। |

**Returns:**
boolean - यदि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है तो true लौटाता है; अन्यथा false।
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| obj | java.lang.Object | इस इंस्टेंस से तुलना करने के लिए निर्दिष्ट ऑब्जेक्ट। |

**Returns:**
boolean - यदि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है तो true लौटाता है; अन्यथा false।
### getBaselineNumber() {#getBaselineNumber--}
```
public final int getBaselineNumber()
```


बेसलाइन डेटा रिकॉर्ड की अद्वितीय संख्या प्राप्त करता है।

**Returns:**
int - बेसलाइन डेटा रिकॉर्ड की विशिष्ट संख्या।
### getBcwp() {#getBcwp--}
```
public final double getBcwp()
```


किसी संसाधन द्वारा किसी परियोजना के लिए अब तक किए गए कार्य की बजटेड लागत प्राप्त करता है।

**Returns:**
double - किसी संसाधन द्वारा किसी परियोजना के लिए अब तक किए गए कार्य की बजटेड लागत।
### getBcws() {#getBcws--}
```
public final double getBcws()
```


संसाधन के लिए निर्धारित कार्य की बजट लागत प्राप्त करता है।

**Returns:**
double - संसाधन के लिए निर्धारित कार्य की बजट लागत।
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


जब बेसलाइन सहेजी जाती है, तब संसाधन की अनुमानित लागत प्राप्त करता है।

**Returns:**
java.math.BigDecimal - जब बेसलाइन सहेजी जाती है, तब संसाधन की अनुमानित लागत।
### getWork() {#getWork--}
```
public final Duration getWork()
```


जब बेसलाइन सहेजी जाती है, तब संसाधन को सौंपे गए कार्य को प्राप्त करता है।

मान: जब बेसलाइन सहेजी गई थी, तब संसाधन को सौंपे गए कार्य की मात्रा।

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the work assigned to a resource when the baseline is saved.
### hashCode() {#hashCode--}
```
public int hashCode()
```


बेसलाइन के लिए हैश कोड मान लौटाता है।

**Returns:**
int - इस ऑब्जेक्ट के लिए हैश कोड मान लौटाता है।
### op_Equality(Baseline a, Baseline b) {#op-Equality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_Equality(Baseline a, Baseline b)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | पहला बेसलाइन। |
| b | [Baseline](../../com.aspose.tasks/baseline) | दूसरा बेसलाइन। |

**Returns:**
boolean - वह मान जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं
### op_GreaterThan(Baseline a, Baseline b) {#op-GreaterThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_GreaterThan(Baseline a, Baseline b)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से बड़ा है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | पहला बेसलाइन। |
| b | [Baseline](../../com.aspose.tasks/baseline) | दूसरा बेसलाइन। |

**Returns:**
boolean - वह मान जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से बड़ा है या नहीं
### op_GreaterThanOrEqual(Baseline a, Baseline b) {#op-GreaterThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_GreaterThanOrEqual(Baseline a, Baseline b)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से बड़ा या बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | पहला बेसलाइन। |
| b | [Baseline](../../com.aspose.tasks/baseline) | दूसरा बेसलाइन। |

**Returns:**
boolean - वह मान जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से बड़ा या बराबर है या नहीं
### op_Inequality(Baseline a, Baseline b) {#op-Inequality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_Inequality(Baseline a, Baseline b)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर नहीं है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | पहला बेसलाइन। |
| b | [Baseline](../../com.aspose.tasks/baseline) | दूसरा बेसलाइन। |

**Returns:**
boolean - वह मान जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर नहीं है या नहीं
### op_LessThan(Baseline a, Baseline b) {#op-LessThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_LessThan(Baseline a, Baseline b)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से छोटा है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | पहला बेसलाइन। |
| b | [Baseline](../../com.aspose.tasks/baseline) | दूसरा बेसलाइन। |

**Returns:**
boolean - वह मान जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से छोटा है या नहीं
### op_LessThanOrEqual(Baseline a, Baseline b) {#op-LessThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_LessThanOrEqual(Baseline a, Baseline b)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से छोटा या बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | पहला बेसलाइन। |
| b | [Baseline](../../com.aspose.tasks/baseline) | दूसरा बेसलाइन। |

**Returns:**
boolean - वह मान जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट से छोटा या बराबर है या नहीं
### setBaselineNumber(int value) {#setBaselineNumber-int-}
```
public final void setBaselineNumber(int value)
```


बेसलाइन डेटा रिकॉर्ड की विशिष्ट संख्या सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | int | बेसलाइन डेटा रिकॉर्ड की विशिष्ट संख्या। |

### setBcwp(double value) {#setBcwp-double-}
```
public final void setBcwp(double value)
```


किसी संसाधन द्वारा किसी परियोजना के लिए अब तक किए गए कार्य की बजटेड लागत सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | double | किसी संसाधन द्वारा किसी परियोजना के लिए अब तक किए गए कार्य की बजटेड लागत। |

### setBcws(double value) {#setBcws-double-}
```
public final void setBcws(double value)
```


संसाधन के लिए निर्धारित कार्य की बजट लागत सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | double | संसाधन के लिए निर्धारित कार्य की बजट लागत। |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


जब बेसलाइन सहेजी जाती है, तब संसाधन की अनुमानित लागत सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.math.BigDecimal | जब बेसलाइन सहेजी जाती है, तब संसाधन की अनुमानित लागत। |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


जब बेसलाइन सहेजी जाती है, तब संसाधन को सौंपे गए कार्य को सेट करता है।

मान: जब बेसलाइन सहेजी गई थी, तब संसाधन को सौंपे गए कार्य की मात्रा।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | जब बेसलाइन सहेजी जाती है, तब संसाधन को सौंपे गए कार्य। |

