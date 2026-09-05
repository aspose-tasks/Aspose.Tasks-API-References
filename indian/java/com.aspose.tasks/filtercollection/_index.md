---
title: "FilterCollection"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "ऑब्जेक्ट्स की एक सूची शामिल करता है।"
type: docs
weight: 92
url: /hi/java/com.aspose.tasks/filtercollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class FilterCollection extends AbstractCollection<Filter>
```

एक सूची में [Filter](../../com.aspose.tasks/filter) ऑब्जेक्ट्स को शामिल करता है। ICollection&lt;Filter&gt; इंटरफ़ेस को लागू करता है।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [add(Filter item)](#add-com.aspose.tasks.Filter-) |  |
| [clear()](#clear--) | इस संग्रह से सभी तत्वों को हटाता है (वैकल्पिक ऑपरेशन)। |
| [contains(Filter item)](#contains-com.aspose.tasks.Filter-) | यदि यह संग्रह निर्दिष्ट आइटम को शामिल करता है तो true लौटाता है। |
| [copyTo(Filter[] array, int arrayIndex)](#copyTo-com.aspose.tasks.Filter---int-) | निर्दिष्ट एरे से तत्वों को इस संग्रह में निर्दिष्ट इंडेक्स से शुरू करके कॉपी करता है। |
| [iterator()](#iterator--) | इस संग्रह में मौजूद तत्वों पर एक इटररेटर लौटाता है। |
| [remove(Filter item)](#remove-com.aspose.tasks.Filter-) | इस संग्रह से निर्दिष्ट आइटम को हटाता है। |
| [size()](#size--) | इस संग्रह में शामिल तत्वों की संख्या प्राप्त करता है। |
| [toList()](#toList--) | फ़िल्टर संग्रह को `Filter` ऑब्जेक्ट्स की सूची में परिवर्तित करता है। |
### add(Filter item) {#add-com.aspose.tasks.Filter-}
```
public boolean add(Filter item)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) |  |

**Returns:**
boolean
### clear() {#clear--}
```
public void clear()
```


इस संग्रह से सभी तत्वों को हटाता है (वैकल्पिक ऑपरेशन)।

### contains(Filter item) {#contains-com.aspose.tasks.Filter-}
```
public final boolean contains(Filter item)
```


यदि यह संग्रह निर्दिष्ट आइटम को शामिल करता है तो true लौटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) | निर्दिष्ट आइटम। |

**Returns:**
boolean - true यदि संग्रह निर्दिष्ट आइटम को शामिल करता है।
### copyTo(Filter[] array, int arrayIndex) {#copyTo-com.aspose.tasks.Filter---int-}
```
public final void copyTo(Filter[] array, int arrayIndex)
```


निर्दिष्ट एरे से तत्वों को इस संग्रह में निर्दिष्ट इंडेक्स से शुरू करके कॉपी करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| array | [Filter\[\]](../../com.aspose.tasks/filter) | तत्वों को कॉपी करने के लिए निर्दिष्ट एक-आयामी एरे। |
| arrayIndex | int | निर्दिष्ट एरे का शून्य-आधारित सूचकांक जहाँ प्रतिलिपि शुरू होती है। |

### iterator() {#iterator--}
```
public Iterator<Filter> iterator()
```


इस संग्रह में मौजूद तत्वों पर एक इटररेटर लौटाता है।

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Filter&gt; - संग्रह इटरेटर।
### remove(Filter item) {#remove-com.aspose.tasks.Filter-}
```
public final boolean remove(Filter item)
```


इस संग्रह से निर्दिष्ट आइटम को हटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) | निर्दिष्ट आइटम। |

**Returns:**
boolean - यदि ऑपरेशन सफल रहा तो true।
### size() {#size--}
```
public final int size()
```


इस संग्रह में शामिल तत्वों की संख्या प्राप्त करता है।

**Returns:**
int - इस संग्रह में शामिल तत्वों की संख्या।
### toList() {#toList--}
```
public List<Filter> toList()
```


फ़िल्टर संग्रह को `Filter` ऑब्जेक्ट्स की सूची में परिवर्तित करता है।

**Returns:**
java.util.List&lt;com.aspose.tasks.Filter&gt; - `Filter` ऑब्जेक्ट्स की सामान्य सूची।
