---
title: "RiskItemStatisticsCollection"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "क्लास की इंस्टेंस को सम्मिलित करने वाला संग्रह दर्शाता है।"
type: docs
weight: 266
url: /hi/java/com.aspose.tasks/riskitemstatisticscollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.util.Map, java.lang.Iterable
```
public class RiskItemStatisticsCollection implements Map<Task,RiskItemStatistics>, Iterable<RiskItemStatistics>
```

एक संग्रह का प्रतिनिधित्व करता है जिसमें [RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) क्लास की इंस्टेंसें शामिल हैं।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [clear()](#clear--) | संग्रह से सभी आइटम हटाता है। |
| [containsKey(Object key)](#containsKey-java.lang.Object-) | यदि इस मैप में निर्दिष्ट कुंजी के लिए मैपिंग मौजूद है तो true लौटाता है। |
| [containsValue(Object value)](#containsValue-java.lang.Object-) | यदि इस मैप में एक या अधिक कुंजियों को निर्दिष्ट मान से मैप किया गया है तो true लौटाता है। |
| [entrySet()](#entrySet--) | इस मैप में मौजूद मैपिंग्स का Set दृश्य लौटाता है। |
| [get(Object task)](#get-java.lang.Object-) | `RiskItemStatistics` क्लास की एक इंस्टेंस लौटाता है जो इस संग्रह में मौजूद है और निर्दिष्ट Task ऑब्जेक्ट से जुड़ी है; यदि आइटम नहीं मिला तो null लौटाता है। |
| [isEmpty()](#isEmpty--) | यदि इस मैप में कोई कुंजी-मूल्य मैपिंग नहीं है तो true लौटाता है। |
| [iterator()](#iterator--) | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [keySet()](#keySet--) | इस मैप में मौजूद कुंजियों का Set दृश्य लौटाता है। |
| [put(Task key, RiskItemStatistics value)](#put-com.aspose.tasks.Task-com.aspose.tasks.RiskItemStatistics-) | निर्दिष्ट मान को इस मैप में निर्दिष्ट कुंजी के साथ जोड़ता है। |
| [putAll(Map&lt;? extends Task,? extends RiskItemStatistics&gt; m)](#putAll-java.util.Map---extends-com.aspose.tasks.Task---extends-com.aspose.tasks.RiskItemStatistics--) | निर्दिष्ट मैप से सभी मैपिंग्स को इस मैप में कॉपी करता है। |
| [remove(Object key)](#remove-java.lang.Object-) | यदि मौजूद हो तो इस मैप से किसी कुंजी की मैपिंग हटाता है। |
| [size()](#size--) | इस संग्रह में तत्वों की संख्या लौटाता है। |
| [values()](#values--) | इस मैप में मौजूद मानों का Collection दृश्य लौटाता है। |
### clear() {#clear--}
```
public void clear()
```


संग्रह से सभी आइटम हटाता है।

### containsKey(Object key) {#containsKey-java.lang.Object-}
```
public boolean containsKey(Object key)
```


यदि इस मैप में निर्दिष्ट कुंजी के लिए मैपिंग मौजूद है तो true लौटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| कुंजी | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - यदि इस मैप में निर्दिष्ट कुंजी के लिए मैपिंग मौजूद है तो true।
### containsValue(Object value) {#containsValue-java.lang.Object-}
```
public boolean containsValue(Object value)
```


यदि इस मैप में एक या अधिक कुंजियों को निर्दिष्ट मान से मैप किया गया है तो true लौटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - यदि इस मैप में एक या अधिक कुंजियों को निर्दिष्ट मान से मैप किया गया है तो true।
### entrySet() {#entrySet--}
```
public Set<Map.Entry<Task,RiskItemStatistics>> entrySet()
```


इस मैप में मौजूद मैपिंग्स का Set दृश्य लौटाता है।

**Returns:**
java.util.Set&lt;java.util.Map.Entry&lt;com.aspose.tasks.Task,com.aspose.tasks.RiskItemStatistics&gt;&gt; - \{@inheritDoc\}
### get(Object task) {#get-java.lang.Object-}
```
public RiskItemStatistics get(Object task)
```


`RiskItemStatistics` क्लास की एक इंस्टेंस लौटाता है जो इस संग्रह में मौजूद है और निर्दिष्ट Task ऑब्जेक्ट से जुड़ी है; यदि आइटम नहीं मिला तो null लौटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| task | java.lang.Object | `Task` क्लास की निर्दिष्ट इंस्टेंस। |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - risk item which is associated with the specified task object if found; null otherwise.
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


यदि इस मैप में कोई कुंजी-मूल्य मैपिंग नहीं है तो true लौटाता है।

**Returns:**
boolean - सही यदि यह मानचित्र कोई कुंजी‑मूल्य मैपिंग नहीं रखता है
### iterator() {#iterator--}
```
public Iterator<RiskItemStatistics> iterator()
```


इस संग्रह के लिए एक एन्यूमरेटर लौटाता है।

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.RiskItemStatistics&gt; - इस संग्रह के लिए एक इटररेटर।
### keySet() {#keySet--}
```
public Set<Task> keySet()
```


इस मैप में मौजूद कुंजियों का Set दृश्य लौटाता है।

**Returns:**
java.util.Set&lt;com.aspose.tasks.Task&gt; - इस मानचित्र में मौजूद कुंजियों का सेट दृश्य।
### put(Task key, RiskItemStatistics value) {#put-com.aspose.tasks.Task-com.aspose.tasks.RiskItemStatistics-}
```
public RiskItemStatistics put(Task key, RiskItemStatistics value)
```


निर्दिष्ट मान को इस मैप में निर्दिष्ट कुंजी के साथ जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| key | [Task](../../com.aspose.tasks/task) | \{@inheritDoc\} |
| value | [RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) | \{@inheritDoc\} |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - \{@inheritDoc\}
### putAll(Map&lt;? extends Task,? extends RiskItemStatistics&gt; m) {#putAll-java.util.Map---extends-com.aspose.tasks.Task---extends-com.aspose.tasks.RiskItemStatistics--}
```
public void putAll(Map<? extends Task,? extends RiskItemStatistics> m)
```


निर्दिष्ट मैप से सभी मैपिंग्स को इस मैप में कॉपी करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| m | java.util.Map&lt;? extends com.aspose.tasks.Task,? extends com.aspose.tasks.RiskItemStatistics&gt; | \{@inheritDoc\} |

### remove(Object key) {#remove-java.lang.Object-}
```
public RiskItemStatistics remove(Object key)
```


यदि मौजूद हो तो इस मैप से किसी कुंजी की मैपिंग हटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| कुंजी | java.lang.Object | \{@inheritDoc\} |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - \{@inheritDoc\}
### size() {#size--}
```
public int size()
```


इस संग्रह में तत्वों की संख्या लौटाता है।

**Returns:**
int - इस संग्रह में तत्वों की संख्या।
### values() {#values--}
```
public Collection<RiskItemStatistics> values()
```


इस मैप में मौजूद मानों का Collection दृश्य लौटाता है।

**Returns:**
java.util.Collection&lt;com.aspose.tasks.RiskItemStatistics&gt; - इस मानचित्र में मौजूद मानों का संग्रह दृश्य।
