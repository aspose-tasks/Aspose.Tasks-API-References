---
title: "Duration"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "परियोजना में अवधि को दर्शाता है।"
type: docs
weight: 76
url: /hi/java/com.aspose.tasks/duration/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public class Duration extends Struct<Duration> implements System.IEquatable<Duration>
```

परियोजना में अवधि को दर्शाता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [Duration()](#Duration--) | निर्दिष्ट TimeSpan मान और TimeUnitType के साथ [Duration](../../com.aspose.tasks/duration) संरचना का नया उदाहरण आरंभ करता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [Clone()](#Clone--) | इस उदाहरण की एक डीप कॉपी बनाता और लौटाता है। |
| [CloneTo(Duration that)](#CloneTo-com.aspose.tasks.Duration-) | उदाहरण की एक डीप कॉपी बनाकर उसे दूसरे उदाहरण में रखता है। |
| [add(Duration d)](#add-com.aspose.tasks.Duration-) | निर्दिष्ट अवधि को इस अवधि में जोड़ता है। |
| [add(double val)](#add-double-) | निर्दिष्ट डबल मान को इस अवधि में जोड़ता है। |
| [clone()](#clone--) | \{@inheritDoc\} |
| [convert(byte timeUnitType)](#convert-byte-) | Duration ऑब्जेक्ट को निर्दिष्ट समय इकाइयों के साथ दूसरी अवधि में परिवर्तित करता है। |
| [equals(Duration other)](#equals-com.aspose.tasks.Duration-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| [equals(Duration obj1, Duration obj2)](#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | एक मान लौटाता है जो दर्शाता है कि निर्दिष्ट `obj1` उदाहरण `obj2` उदाहरण के बराबर है या नहीं। |
| [equals(Object obj)](#equals-java.lang.Object-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| [getTimeSpan()](#getTimeSpan--) | इस Duration ऑब्जेक्ट की `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) इंस्टेंस प्राप्त करता है। |
| [getTimeUnit()](#getTimeUnit--) | इस वस्तु के लिए समय इकाई प्रकार प्राप्त करता है। |
| [hashCode()](#hashCode--) | इस वस्तु के लिए हैश कोड मान लौटाता है। |
| [isElapsed()](#isElapsed--) | समय इकाई समाप्त हुई है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [isEstimated()](#isEstimated--) | समय इकाई अनुमानित है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [op_Equality(Duration a, Duration b)](#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| [op_Inequality(Duration a, Duration b)](#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर नहीं है या नहीं। |
| [parse(Project p, String value)](#parse-com.aspose.tasks.Project-java.lang.String-) | निर्दिष्ट स्ट्रिंग को [Duration](../../com.aspose.tasks/duration) संरचना के उदाहरण में परिवर्तित करता है। |
| [parseTimeSpan(String value)](#parseTimeSpan-java.lang.String-) | फ़ॉर्मेट "PT--H--M--S--" में अवधि स्ट्रिंग को पार्स करता है। |
| [subtract(Duration d)](#subtract-com.aspose.tasks.Duration-) | इस अवधि उदाहरण से निर्दिष्ट अवधि घटाता है। |
| [subtract(double val)](#subtract-double-) | इस अवधि उदाहरण से निर्दिष्ट डबल मान घटाता है। |
| [toDouble()](#toDouble--) | Duration ऑब्जेक्ट को `double` मान में परिवर्तित करता है। |
| [toString()](#toString--) | इस उदाहरण का स्ट्रिंग प्रतिनिधित्व लौटाता है। |
### Duration() {#Duration--}
```
public Duration()
```


निर्दिष्ट TimeSpan मान और TimeUnitType के साथ [Duration](../../com.aspose.tasks/duration) संरचना का नया उदाहरण आरंभ करता है।

### Clone() {#Clone--}
```
public Duration Clone()
```


इस उदाहरण की एक डीप कॉपी बनाता और लौटाता है।

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a deep copy of this object.
### CloneTo(Duration that) {#CloneTo-com.aspose.tasks.Duration-}
```
public void CloneTo(Duration that)
```


उदाहरण की एक डीप कॉपी बनाकर उसे दूसरे उदाहरण में रखता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| that | [Duration](../../com.aspose.tasks/duration) | एक अन्य उदाहरण। |

### add(Duration d) {#add-com.aspose.tasks.Duration-}
```
public final Duration add(Duration d)
```


निर्दिष्ट अवधि को इस अवधि में जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | इस उदाहरण में जोड़ने के लिए निर्दिष्ट [Duration](../../com.aspose.tasks/duration)। |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance plus the specified duration value.
### add(double val) {#add-double-}
```
public final Duration add(double val)
```


निर्दिष्ट डबल मान को इस अवधि में जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | double | इस उदाहरण में जोड़ने के लिए निर्दिष्ट `double` मान। |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance plus the specified duration value.
### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
### convert(byte timeUnitType) {#convert-byte-}
```
public final Duration convert(byte timeUnitType)
```


Duration ऑब्जेक्ट को निर्दिष्ट समय इकाइयों के साथ दूसरी अवधि में परिवर्तित करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| timeUnitType | byte | निर्दिष्ट समय इकाई प्रकार। |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - returns new duration with the specified unit type.
### equals(Duration other) {#equals-com.aspose.tasks.Duration-}
```
public final boolean equals(Duration other)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| other | [Duration](../../com.aspose.tasks/duration) | इस इंस्टेंस की तुलना करने के लिए ऑब्जेक्ट। |

**Returns:**
बूलियन - **True** लौटाता है यदि अन्य Duration उदाहरण के पास इस उदाहरण के समान TimeSpan और TimeUnit मान हैं; अन्यथा, **false**।
### equals(Duration obj1, Duration obj2) {#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean equals(Duration obj1, Duration obj2)
```


एक मान लौटाता है जो दर्शाता है कि निर्दिष्ट `obj1` उदाहरण `obj2` उदाहरण के बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| obj1 | [Duration](../../com.aspose.tasks/duration) | तुलना करने के लिए पहला ऑब्जेक्ट। |
| obj2 | [Duration](../../com.aspose.tasks/duration) | तुलना करने के लिए दूसरा ऑब्जेक्ट। |

**Returns:**
boolean - यदि निर्दिष्ट `obj1` उदाहरण निर्दिष्ट `obj2` उदाहरण के बराबर है तो true लौटाता है; अन्यथा false।
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| obj | java.lang.Object | इस इंस्टेंस की तुलना करने के लिए ऑब्जेक्ट। |

**Returns:**
बूलियन - **True** यदि निर्दिष्ट ऑब्जेक्ट एक Duration है जिसके पास इस उदाहरण के समान TimeSpan और TimeUnit मान हैं; अन्यथा, **false**।
### getTimeSpan() {#getTimeSpan--}
```
public final double getTimeSpan()
```


इस Duration ऑब्जेक्ट की `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) इंस्टेंस प्राप्त करता है।

मान: इस Duration ऑब्जेक्ट का TimeSpan उदाहरण।

**Returns:**
डबल - `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) इस Duration ऑब्जेक्ट का उदाहरण।
### getTimeUnit() {#getTimeUnit--}
```
public final byte getTimeUnit()
```


इस वस्तु के लिए समय इकाई प्रकार प्राप्त करता है।

मान: इस Duration उदाहरण का समय इकाई प्रकार।

**Returns:**
बाइट - इस वस्तु के लिए समय इकाई प्रकार।
### hashCode() {#hashCode--}
```
public int hashCode()
```


इस वस्तु के लिए हैश कोड मान लौटाता है।

**Returns:**
इंट - इस अवधि उदाहरण के लिए हैश कोड मान लौटाता है।
### isElapsed() {#isElapsed--}
```
public final boolean isElapsed()
```


समय इकाई समाप्त हुई है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

मान: वह फ़्लैग जो निर्धारित करता है कि यह Duration उदाहरण समाप्त हुआ है या नहीं।

**Returns:**
बूलियन - एक मान जो दर्शाता है कि समय इकाई समाप्त हुई है या नहीं।
### isEstimated() {#isEstimated--}
```
public final boolean isEstimated()
```


समय इकाई अनुमानित है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

मान: वह फ़्लैग जो निर्धारित करता है कि यह Duration उदाहरण अनुमानित है या नहीं।

**Returns:**
बूलियन - एक मान जो दर्शाता है कि समय इकाई अनुमानित है या नहीं।
### op_Equality(Duration a, Duration b) {#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Equality(Duration a, Duration b)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | पहली अवधि। |
| b | [Duration](../../com.aspose.tasks/duration) | दूसरी अवधि। |

**Returns:**
boolean - वह मान जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं
### op_Inequality(Duration a, Duration b) {#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Inequality(Duration a, Duration b)
```


एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर नहीं है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | पहली अवधि। |
| b | [Duration](../../com.aspose.tasks/duration) | दूसरी अवधि। |

**Returns:**
boolean - वह मान जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर नहीं है या नहीं
### parse(Project p, String value) {#parse-com.aspose.tasks.Project-java.lang.String-}
```
public static Duration parse(Project p, String value)
```


निर्दिष्ट स्ट्रिंग को [Duration](../../com.aspose.tasks/duration) संरचना के उदाहरण में परिवर्तित करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| p | [Project](../../com.aspose.tasks/project) | निर्दिष्ट [Project](../../com.aspose.tasks/project) वर्ग की वह उदाहरण जिसके लिए अवधि को परिवर्तित किया जाना है। |
| मान | java.lang.String | निर्दिष्ट स्ट्रिंग जिसे परिवर्तित किया जाना है। |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Returns the converted instance of [Duration](../../com.aspose.tasks/duration) struct.
### parseTimeSpan(String value) {#parseTimeSpan-java.lang.String-}
```
public static double parseTimeSpan(String value)
```


फ़ॉर्मेट "PT--H--M--S--" में अवधि स्ट्रिंग को पार्स करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | निर्दिष्ट स्ट्रिंग जिसे पार्स किया जाना है। |

**Returns:**
double - `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) संरचना का पार्स किया गया उदाहरण लौटाता है।
### subtract(Duration d) {#subtract-com.aspose.tasks.Duration-}
```
public final Duration subtract(Duration d)
```


इस अवधि उदाहरण से निर्दिष्ट अवधि घटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | इस उदाहरण से घटाने के लिए निर्दिष्ट [Duration](../../com.aspose.tasks/duration) उदाहरण। |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### subtract(double val) {#subtract-double-}
```
public final Duration subtract(double val)
```


इस अवधि उदाहरण से निर्दिष्ट डबल मान घटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | double | इस उदाहरण से घटाने के लिए निर्दिष्ट `double` मान। |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### toDouble() {#toDouble--}
```
public final double toDouble()
```


Duration ऑब्जेक्ट को `double` मान में परिवर्तित करता है।

**Returns:**
double - परिवर्तित मान।
### toString() {#toString--}
```
public String toString()
```


इस उदाहरण का स्ट्रिंग प्रतिनिधित्व लौटाता है।

**Returns:**
java.lang.String - इस उदाहरण का स्ट्रिंग प्रतिनिधित्व।
