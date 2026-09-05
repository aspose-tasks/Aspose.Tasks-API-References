---
title: "TimeDelta"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "दो टाइमस्टैम्प के बीच अंतर का प्रतिनिधित्व करता है।"
type: docs
weight: 317
url: /hi/java/com.aspose.tasks/timedelta/
---

**Inheritance:**
java.lang.Object
```
public class TimeDelta
```

दो टाइमस्टैम्प के बीच अंतर का प्रतिनिधित्व करता है।
## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [TimeDelta(int hours, int minutes, int seconds)](#TimeDelta-int-int-int-) | निर्दिष्ट घंटे, मिनट और सेकंड की संख्या के साथ TimeDelta का नया उदाहरण प्रारंभ करता है। |
| [TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)](#TimeDelta-int-int-int-int-int-) | निर्दिष्ट दिन, घंटे, मिनट, सेकंड और मिलीसेकंड की संख्या के साथ TimeDelta का नया उदाहरण प्रारंभ करता है। |
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [add(TimeDelta other)](#add-com.aspose.tasks.TimeDelta-) | एक नया TimeDelta वस्तु लौटाता है जिसका मान इस और अन्य उदाहरण का योग है। |
| [clone()](#clone--) | \{@inheritDoc\} |
| [compare(TimeDelta t1, TimeDelta t2)](#compare-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | दो TimeDelta मानों की तुलना करता है और एक पूर्णांक लौटाता है जो दर्शाता है कि पहला मान दूसरे मान से छोटा, बराबर या बड़ा है। |
| [compareTo(TimeDelta other)](#compareTo-com.aspose.tasks.TimeDelta-) | इस उदाहरण की तुलना निर्दिष्ट TimeDelta वस्तु से करता है और एक पूर्णांक लौटाता है जो दर्शाता है कि यह उदाहरण TimeSpan वस्तु से छोटा, बराबर या बड़ा है। |
| [equals(TimeDelta other)](#equals-com.aspose.tasks.TimeDelta-) | `other` समय अंतराल इस के बराबर है या नहीं, दर्शाता है। |
| [equals(TimeDelta t1, TimeDelta t2)](#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-) | दो उदाहरणों की समानता की जाँच करता है। |
| [equals(Object other)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [fromDays(double value)](#fromDays-double-) | एक TimeDelta लौटाता है जो निर्दिष्ट संख्या में दिनों को दर्शाता है (निकटतम मिलीसेकंड तक गोल किया गया)। |
| [fromHours(double value)](#fromHours-double-) | एक TimeDelta लौटाता है जो निर्दिष्ट संख्या में घंटों को दर्शाता है (निकटतम मिलीसेकंड तक गोल किया गया)। |
| [fromMilliseconds(double value)](#fromMilliseconds-double-) | एक TimeDelta लौटाता है जो निर्दिष्ट संख्या में मिलीसेकंड को दर्शाता है (निकटतम मिलीसेकंड तक गोल किया गया)। |
| [fromMinutes(double value)](#fromMinutes-double-) | एक TimeDelta लौटाता है जो निर्दिष्ट संख्या में मिनटों को दर्शाता है (निकटतम मिलीसेकंड तक गोल किया गया)। |
| [fromSeconds(double value)](#fromSeconds-double-) | एक TimeDelta लौटाता है जो निर्दिष्ट संख्या में सेकंड को दर्शाता है (निकटतम मिलीसेकंड तक गोल किया गया)। |
| [getDays()](#getDays--) | इस उदाहरण द्वारा प्रतिनिधित्व किए गए समय अंतराल का दिन घटक लौटाता है। |
| [getHours()](#getHours--) | इस उदाहरण द्वारा प्रतिनिधित्व किए गए समय अंतराल का घंटा घटक लौटाता है। |
| [getMilliseconds()](#getMilliseconds--) | इस उदाहरण द्वारा प्रतिनिधित्व किए गए समय अंतराल का मिलीसेकंड घटक लौटाता है। |
| [getMinutes()](#getMinutes--) | इस उदाहरण द्वारा प्रतिनिधित्व किए गए समय अंतराल का मिनट घटक लौटाता है। |
| [getSeconds()](#getSeconds--) | इस उदाहरण द्वारा प्रतिनिधित्व किए गए समय अंतराल का सेकंड घटक लौटाता है। |
| [getTotalDays()](#getTotalDays--) | वर्तमान उदाहरण का मान पूर्ण और अंशीय दिनों में व्यक्त करके लौटाता है। |
| [getTotalHours()](#getTotalHours--) | वर्तमान उदाहरण का मान पूर्ण और अंशीय घंटों में व्यक्त करके लौटाता है। |
| [getTotalMilliseconds()](#getTotalMilliseconds--) | वर्तमान उदाहरण का मान पूर्ण और अंशीय मिलीसेकंड में व्यक्त करके लौटाता है। |
| [getTotalMinutes()](#getTotalMinutes--) | वर्तमान उदाहरण का मान पूर्ण और अंशीय मिनटों में व्यक्त करके लौटाता है। |
| [getTotalSeconds()](#getTotalSeconds--) | वर्तमान उदाहरण का मान पूर्ण और अंशीय सेकंड में व्यक्त करके लौटाता है। |
| [hashCode()](#hashCode--) | \{@inheritDoc\} |
| [negate()](#negate--) | एक नया `TimeDelta` लौटाता है जिसका मान इस उदाहरण के नकारात्मक मान के बराबर है। |
| [parse(String s)](#parse-java.lang.String-) | समय अंतराल की स्ट्रिंग प्रतिनिधित्व को उसके `TimeDelta` समकक्ष में बदलता है। |
| [subtract(TimeDelta other)](#subtract-com.aspose.tasks.TimeDelta-) | एक नया TimeDelta ऑब्जेक्ट लौटाता है जिसका मान इस और `other` उदाहरणों के बीच का अंतर है। |
| [toString()](#toString--) | \{@inheritDoc\} |
| [tryParse(String s, TimeDelta[] result)](#tryParse-java.lang.String-com.aspose.tasks.TimeDelta---) | समय अंतराल की स्ट्रिंग प्रतिनिधित्व को उसके TimeDelta समकक्ष में बदलता है और एक मान लौटाता है जो दर्शाता है कि रूपांतरण सफल हुआ या नहीं। |
### TimeDelta(int hours, int minutes, int seconds) {#TimeDelta-int-int-int-}
```
public TimeDelta(int hours, int minutes, int seconds)
```


निर्दिष्ट घंटे, मिनट और सेकंड की संख्या के साथ TimeDelta का नया उदाहरण प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| घंटे | int | घंटों की संख्या। |
| मिनट | int | मिनटों की संख्या। |
| सेकंड | int | सेकंड की संख्या। |

### TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds) {#TimeDelta-int-int-int-int-int-}
```
public TimeDelta(int days, int hours, int minutes, int seconds, int milliseconds)
```


निर्दिष्ट दिन, घंटे, मिनट, सेकंड और मिलीसेकंड की संख्या के साथ TimeDelta का नया उदाहरण प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| दिन | int | दिनों की संख्या। |
| घंटे | int | घंटों की संख्या। |
| मिनट | int | मिनटों की संख्या। |
| सेकंड | int | सेकंड की संख्या। |
| मिलीसेकंड | int | मिलीसेकंड की संख्या। |

### add(TimeDelta other) {#add-com.aspose.tasks.TimeDelta-}
```
public TimeDelta add(TimeDelta other)
```


एक नया TimeDelta वस्तु लौटाता है जिसका मान इस और अन्य उदाहरण का योग है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | जिस उदाहरण के साथ जोड़ना है। |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a new object that represents the value of this instance plus value of other instance.
### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
### compare(TimeDelta t1, TimeDelta t2) {#compare-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-}
```
public static int compare(TimeDelta t1, TimeDelta t2)
```


दो TimeDelta मानों की तुलना करता है और एक पूर्णांक लौटाता है जो दर्शाता है कि पहला मान दूसरे मान से छोटा, बराबर या बड़ा है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | तुलना करने के लिए पहला समय अंतराल। |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | तुलना करने के लिए दूसरा समय अंतराल। |

**Returns:**
int - \-1 यदि `t1` `t2` से छोटा है, 0 यदि `t1` `t2` के बराबर है और 1 यदि `t1` `t2` से बड़ा है।
### compareTo(TimeDelta other) {#compareTo-com.aspose.tasks.TimeDelta-}
```
public int compareTo(TimeDelta other)
```


इस उदाहरण की तुलना निर्दिष्ट TimeDelta वस्तु से करता है और एक पूर्णांक लौटाता है जो दर्शाता है कि यह उदाहरण TimeSpan वस्तु से छोटा, बराबर या बड़ा है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | तुलना करने के लिए एक उदाहरण। |

**Returns:**
int - \-1 यदि यह उदाहरण `other` से छोटा है, 0 यदि यह उदाहरण `other` के बराबर है और 1 यदि यह उदाहरण `other` से बड़ा है।
### equals(TimeDelta other) {#equals-com.aspose.tasks.TimeDelta-}
```
public boolean equals(TimeDelta other)
```


`other` समय अंतराल इस के बराबर है या नहीं, दर्शाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | तुलना करने के लिए समय अवधि। |

**Returns:**
boolean - यदि अंतराल समान हैं तो `true`; अन्यथा `false`।
### equals(TimeDelta t1, TimeDelta t2) {#equals-com.aspose.tasks.TimeDelta-com.aspose.tasks.TimeDelta-}
```
public static boolean equals(TimeDelta t1, TimeDelta t2)
```


दो उदाहरणों की समानता की जाँच करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| t1 | [TimeDelta](../../com.aspose.tasks/timedelta) | पहला उदाहरण। |
| t2 | [TimeDelta](../../com.aspose.tasks/timedelta) | दूसरा उदाहरण। |

**Returns:**
boolean - यदि उदाहरण समान हैं तो `true`; अन्यथा `false`।
### equals(Object other) {#equals-java.lang.Object-}
```
public boolean equals(Object other)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| अन्य | java.lang.Object | \{@inheritDoc\} |

**Returns:**
बूलियन - \{@inheritDoc\}
### fromDays(double value) {#fromDays-double-}
```
public static TimeDelta fromDays(double value)
```


एक TimeDelta लौटाता है जो निर्दिष्ट संख्या में दिनों को दर्शाता है (निकटतम मिलीसेकंड तक गोल किया गया)।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | double | दिनों की संख्या। |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromHours(double value) {#fromHours-double-}
```
public static TimeDelta fromHours(double value)
```


एक TimeDelta लौटाता है जो निर्दिष्ट संख्या में घंटों को दर्शाता है (निकटतम मिलीसेकंड तक गोल किया गया)।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | double | घंटों की संख्या। |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMilliseconds(double value) {#fromMilliseconds-double-}
```
public static TimeDelta fromMilliseconds(double value)
```


एक TimeDelta लौटाता है जो निर्दिष्ट संख्या में मिलीसेकंड को दर्शाता है (निकटतम मिलीसेकंड तक गोल किया गया)।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | double | मिलीसेकंड की संख्या। |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromMinutes(double value) {#fromMinutes-double-}
```
public static TimeDelta fromMinutes(double value)
```


एक TimeDelta लौटाता है जो निर्दिष्ट संख्या में मिनटों को दर्शाता है (निकटतम मिलीसेकंड तक गोल किया गया)।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | double | मिनटों की संख्या। |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### fromSeconds(double value) {#fromSeconds-double-}
```
public static TimeDelta fromSeconds(double value)
```


एक TimeDelta लौटाता है जो निर्दिष्ट संख्या में सेकंड को दर्शाता है (निकटतम मिलीसेकंड तक गोल किया गया)।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | double | सेकंड की संख्या। |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - an object that represents `value`.
### getDays() {#getDays--}
```
public int getDays()
```


इस उदाहरण द्वारा प्रतिनिधित्व किए गए समय अंतराल का दिन घटक लौटाता है।

**Returns:**
int - समय अंतराल का दिन घटक। यह सकारात्मक या नकारात्मक हो सकता है।
### getHours() {#getHours--}
```
public int getHours()
```


इस उदाहरण द्वारा प्रतिनिधित्व किए गए समय अंतराल का घंटा घटक लौटाता है।

**Returns:**
int - समय अंतराल का घंटे घटक, जो -23 से 23 की सीमा में है।
### getMilliseconds() {#getMilliseconds--}
```
public int getMilliseconds()
```


इस उदाहरण द्वारा प्रतिनिधित्व किए गए समय अंतराल का मिलीसेकंड घटक लौटाता है।

**Returns:**
int - समय अंतराल का मिलीसेकंड घटक, जो -999 से 999 की सीमा में है।
### getMinutes() {#getMinutes--}
```
public int getMinutes()
```


इस उदाहरण द्वारा प्रतिनिधित्व किए गए समय अंतराल का मिनट घटक लौटाता है।

**Returns:**
int - समय अंतराल के मिनट घटक का मान, जो -59 से 59 की सीमा में है।
### getSeconds() {#getSeconds--}
```
public int getSeconds()
```


इस उदाहरण द्वारा प्रतिनिधित्व किए गए समय अंतराल का सेकंड घटक लौटाता है।

**Returns:**
int - समय अंतराल के सेकंड घटक का मान, जो -59 से 59 की सीमा में है।
### getTotalDays() {#getTotalDays--}
```
public double getTotalDays()
```


वर्तमान उदाहरण का मान पूर्ण और अंशीय दिनों में व्यक्त करके लौटाता है।

**Returns:**
double - इस उदाहरण द्वारा दर्शाए गए कुल दिनों की संख्या।
### getTotalHours() {#getTotalHours--}
```
public double getTotalHours()
```


वर्तमान उदाहरण का मान पूर्ण और अंशीय घंटों में व्यक्त करके लौटाता है।

**Returns:**
double - इस उदाहरण द्वारा दर्शाए गए कुल घंटों की संख्या।
### getTotalMilliseconds() {#getTotalMilliseconds--}
```
public double getTotalMilliseconds()
```


वर्तमान उदाहरण का मान पूर्ण और अंशीय मिलीसेकंड में व्यक्त करके लौटाता है।

**Returns:**
double - इस उदाहरण द्वारा दर्शाए गए कुल मिलीसेकंड की संख्या।
### getTotalMinutes() {#getTotalMinutes--}
```
public double getTotalMinutes()
```


वर्तमान उदाहरण का मान पूर्ण और अंशीय मिनटों में व्यक्त करके लौटाता है।

**Returns:**
double - इस उदाहरण द्वारा दर्शाए गए कुल मिनटों की संख्या।
### getTotalSeconds() {#getTotalSeconds--}
```
public double getTotalSeconds()
```


वर्तमान उदाहरण का मान पूर्ण और अंशीय सेकंड में व्यक्त करके लौटाता है।

**Returns:**
double - इस उदाहरण द्वारा दर्शाए गए कुल सेकंड की संख्या।
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int - \{@inheritDoc\}
### negate() {#negate--}
```
public TimeDelta negate()
```


एक नया `TimeDelta` लौटाता है जिसका मान इस उदाहरण के नकारात्मक मान के बराबर है।

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - A new object with the same numeric value as this instance, but with the opposite sign.
### parse(String s) {#parse-java.lang.String-}
```
public static TimeDelta parse(String s)
```


समय अंतराल की स्ट्रिंग प्रतिनिधित्व को उसके `TimeDelta` समकक्ष में बदलता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| s | java.lang.String | एक स्ट्रिंग जो परिवर्तित करने के लिए समय अंतराल को निर्दिष्ट करती है। |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a time interval that corresponds to `s`.
### subtract(TimeDelta other) {#subtract-com.aspose.tasks.TimeDelta-}
```
public TimeDelta subtract(TimeDelta other)
```


एक नया TimeDelta ऑब्जेक्ट लौटाता है जिसका मान इस और `other` उदाहरणों के बीच का अंतर है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| other | [TimeDelta](../../com.aspose.tasks/timedelta) | घटाने के लिए उदाहरण। |

**Returns:**
[TimeDelta](../../com.aspose.tasks/timedelta) - a new object that represents the value of this instance minus value of other instance.
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String - \{@inheritDoc\}
### tryParse(String s, TimeDelta[] result) {#tryParse-java.lang.String-com.aspose.tasks.TimeDelta---}
```
public static boolean tryParse(String s, TimeDelta[] result)
```


समय अंतराल की स्ट्रिंग प्रतिनिधित्व को उसके TimeDelta समकक्ष में बदलता है और एक मान लौटाता है जो दर्शाता है कि रूपांतरण सफल हुआ या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| s | java.lang.String | एक स्ट्रिंग जो परिवर्तित करने के लिए समय अंतराल को निर्दिष्ट करती है। |
| result | [TimeDelta\[\]](../../com.aspose.tasks/timedelta) | इस एरे में कम से कम एक तत्व होना चाहिए। जब यह मेथड लौटता है, `result[0]` में वह ऑब्जेक्ट होता है जो `s` द्वारा निर्दिष्ट समय अंतराल को दर्शाता है, या यदि रूपांतरण विफल हो गया तो शून्य-लंबाई का समय अंतराल। |

**Returns:**
boolean - यदि s सफलतापूर्वक परिवर्तित हुआ तो `true`; अन्यथा `false`।
