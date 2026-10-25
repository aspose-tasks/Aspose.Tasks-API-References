---
title: "RateCollection"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "एक संग्रह का प्रतिनिधित्व करता है जिसमें वस्तुएँ होती हैं।"
type: docs
weight: 234
url: /hi/java/com.aspose.tasks/ratecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractMap

**All Implemented Interfaces:**
java.lang.Iterable
```
public class RateCollection extends AbstractMap<Integer,RateByDateCollection> implements Iterable<Map.Entry<Integer,RateByDateCollection>>
```

एक संग्रह का प्रतिनिधित्व करता है जिसमें [Rate](../../com.aspose.tasks/rate) वस्तुएँ होती हैं।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [add(Date ratesFrom)](#add-java.util.Date-) | इस संग्रह में एक नया [Rate](../../com.aspose.tasks/rate) उदाहरण जोड़ता है। |
| [add(Date ratesFrom, int type)](#add-java.util.Date-int-) | इस संग्रह में एक नया [Rate](../../com.aspose.tasks/rate) उदाहरण जोड़ता है। |
| [clear()](#clear--) | \{@inheritDoc\} |
| [entrySet()](#entrySet--) | (@inheritDoc\} |
| [get(Object key)](#get-java.lang.Object-) | (@inheritDoc\} |
| [getByRateType(int key)](#getByRateType-int-) | निर्दिष्ट अनुक्रमांक पर तत्व लौटाता है। |
| [getParentResource()](#getParentResource--) | इस संग्रह के लिए पैरेंट [Resource](../../com.aspose.tasks/resource) ऑब्जेक्ट प्राप्त करता है। |
| [isReadOnly()](#isReadOnly--) | एक मान प्राप्त करता है जो दर्शाता है कि यह संग्रह केवल-पढ़ने योग्य है या नहीं। |
| [iterator()](#iterator--) | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [put(Integer key, RateByDateCollection value)](#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-) | (@inheritDoc\} |
| [remove(Rate item)](#remove-com.aspose.tasks.Rate-) | इस संग्रह से Rate उदाहरण हटाता है। |
| [setByRateType(int key, RateByDateCollection value)](#setByRateType-int-com.aspose.tasks.RateByDateCollection-) | निर्दिष्ट अनुक्रमांक पर तत्व सेट करता है। |
| [size()](#size--) | RateCollection में सम्मिलित तत्वों की संख्या प्राप्त करता है। |
| [toList()](#toList--) | [RateCollection](../../com.aspose.tasks/ratecollection) ऑब्जेक्ट को [Rate](../../com.aspose.tasks/rate) ऑब्जेक्ट्स की सूची में बदलता है। |
| [toList(int type)](#toList-int-) | [RateCollection](../../com.aspose.tasks/ratecollection) ऑब्जेक्ट को निर्दिष्ट [RateType](../../com.aspose.tasks/ratetype) प्रकार द्वारा फ़िल्टर की गई [Rate](../../com.aspose.tasks/rate) ऑब्जेक्ट्स की सूची में बदलता है। |
### add(Date ratesFrom) {#add-java.util.Date-}
```
public final Rate add(Date ratesFrom)
```


इस संग्रह में एक नया [Rate](../../com.aspose.tasks/rate) उदाहरण जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| ratesFrom | java.util.Date | नई दर के प्रभावी होने की तिथि। |

**Returns:**
[Rate](../../com.aspose.tasks/rate) - Added [Rate](../../com.aspose.tasks/rate) instance.
### add(Date ratesFrom, int type) {#add-java.util.Date-int-}
```
public final Rate add(Date ratesFrom, int type)
```


इस संग्रह में एक नया [Rate](../../com.aspose.tasks/rate) उदाहरण जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| ratesFrom | java.util.Date | नई दर के प्रभावी होने की तिथि। |
| प्रकार | int | जिस दर तालिका में जोड़ना है। |

**Returns:**
[Rate](../../com.aspose.tasks/rate) - Added [Rate](../../com.aspose.tasks/rate) instance.
### clear() {#clear--}
```
public final void clear()
```




### entrySet() {#entrySet--}
```
public Set<Map.Entry<Integer,RateByDateCollection>> entrySet()
```


(@inheritDoc\}

**Returns:**
java.util.Set&lt;java.util.Map.Entry&lt;java.lang.Integer,com.aspose.tasks.RateByDateCollection&gt;&gt; - \{@inheritDoc\}
### get(Object key) {#get-java.lang.Object-}
```
public final RateByDateCollection get(Object key)
```


(@inheritDoc\}

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| कुंजी | java.lang.Object | \{@inheritDoc\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### getByRateType(int key) {#getByRateType-int-}
```
public final RateByDateCollection getByRateType(int key)
```


निर्दिष्ट अनुक्रमांक पर तत्व लौटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| कुंजी | int | प्राप्त करने वाले तत्व का शून्य-आधारित अनुक्रमांक। |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - the element at the specified index.
### getParentResource() {#getParentResource--}
```
public final Resource getParentResource()
```


इस संग्रह के लिए पैरेंट [Resource](../../com.aspose.tasks/resource) ऑब्जेक्ट प्राप्त करता है।

**Returns:**
[Resource](../../com.aspose.tasks/resource) - the parent [Resource](../../com.aspose.tasks/resource) object for this collection.
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


एक मान प्राप्त करता है जो दर्शाता है कि यह संग्रह केवल-पढ़ने योग्य है या नहीं।

**Returns:**
boolean - एक मान जो दर्शाता है कि यह संग्रह केवल-पढ़ने योग्य है या नहीं।
### iterator() {#iterator--}
```
public final Iterator iterator()
```


इस संग्रह के लिए एक एन्यूमरेटर लौटाता है।

**Returns:**
java.util.Iterator - इस संग्रह के लिए एक इटरेटर।
### put(Integer key, RateByDateCollection value) {#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-}
```
public final RateByDateCollection put(Integer key, RateByDateCollection value)
```


(@inheritDoc\}

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| कुंजी | java.lang.Integer | \{@inheritDoc\} |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | \{@inheritDoc\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### remove(Rate item) {#remove-com.aspose.tasks.Rate-}
```
public final boolean remove(Rate item)
```


इस संग्रह से Rate उदाहरण हटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| item | [Rate](../../com.aspose.tasks/rate) | हटाने के लिए आइटम। |

**Returns:**
boolean - यदि निर्दिष्ट Rate सफलतापूर्वक हटाया गया हो तो true; अन्यथा false।
### setByRateType(int key, RateByDateCollection value) {#setByRateType-int-com.aspose.tasks.RateByDateCollection-}
```
public final void setByRateType(int key, RateByDateCollection value)
```


निर्दिष्ट अनुक्रमांक पर तत्व सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| कुंजी | int | सेट करने के लिए तत्व का शून्य-आधारित सूचकांक। |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | निर्दिष्ट सूचकांक पर सेट करने के लिए तत्व। |

### size() {#size--}
```
public final int size()
```


RateCollection में सम्मिलित तत्वों की संख्या प्राप्त करता है।

**Returns:**
int - RateCollection में मौजूद तत्वों की संख्या।
### toList() {#toList--}
```
public final List<Rate> toList()
```


[RateCollection](../../com.aspose.tasks/ratecollection) ऑब्जेक्ट को [Rate](../../com.aspose.tasks/rate) ऑब्जेक्ट्स की सूची में बदलता है।

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - [Rate](../../com.aspose.tasks/rate) ऑब्जेक्ट्स की सूची।
### toList(int type) {#toList-int-}
```
public final List<Rate> toList(int type)
```


[RateCollection](../../com.aspose.tasks/ratecollection) ऑब्जेक्ट को निर्दिष्ट [RateType](../../com.aspose.tasks/ratetype) प्रकार द्वारा फ़िल्टर की गई [Rate](../../com.aspose.tasks/rate) ऑब्जेक्ट्स की सूची में बदलता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रकार | int | फ़िल्टर करने के लिए प्रकार। |

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - [Rate](../../com.aspose.tasks/rate) ऑब्जेक्ट्स की एक सूची।
