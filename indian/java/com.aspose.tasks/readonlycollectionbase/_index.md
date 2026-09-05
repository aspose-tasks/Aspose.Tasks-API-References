---
title: "ReadOnlyCollectionBase"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "ऑब्जेक्ट्स का केवल-पढ़ने योग्य संग्रह दर्शाता है।"
type: docs
weight: 238
url: /hi/java/com.aspose.tasks/readonlycollectionbase/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public abstract class ReadOnlyCollectionBase<T> extends AbstractList<T>
```

ऑब्जेक्ट्स का केवल-पढ़ने योग्य संग्रह दर्शाता है।

T : संग्रह आइटम्स का प्रकार।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [add(T item)](#add-T-) | यह ICollection के Add मेथड की स्टब कार्यान्वयन है, जो केवल UnsupportedOperationException फेंकता है। |
| [add(int index, T element)](#add-int-T-) | \{@inheritDoc\} |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | निर्दिष्ट अनुक्रमांक पर तत्व लौटाता है। |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | निर्धारित करता है कि संग्रह केवल‑पढ़ने योग्य है या नहीं। |
| [iterator()](#iterator--) | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [remove(int index)](#remove-int-) | \{@inheritDoc\} |
| [remove(Object o)](#remove-java.lang.Object-) | \{@inheritDoc\} |
| [set(int index, T value)](#set-int-T-) | निर्दिष्ट अनुक्रमांक पर तत्व लौटाता है। |
| [size()](#size--) | ऑब्जेक्ट में सम्मिलित वस्तुओं की संख्या प्राप्त करता है। |
| [toList()](#toList--) | संग्रह को वस्तुओं की सूची में परिवर्तित करता है। |
### add(T item) {#add-T-}
```
public final boolean add(T item)
```


यह ICollection के Add मेथड की स्टब कार्यान्वयन है, जो केवल UnsupportedOperationException फेंकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| item | T | जोड़ने के लिए आइटम। |

**Returns:**
boolean
### add(int index, T element) {#add-int-T-}
```
public final void add(int index, T element)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | \{@inheritDoc\} |
| तत्व | T | \{@inheritDoc\} |

### clear() {#clear--}
```
public final void clear()
```




### contains(Object o) {#contains-java.lang.Object-}
```
public final boolean contains(Object o)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
बूलियन - \{@inheritDoc\}
### get(int index) {#get-int-}
```
public final T get(int index)
```


निर्दिष्ट अनुक्रमांक पर तत्व लौटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | प्राप्त करने वाले तत्व का शून्य-आधारित अनुक्रमांक। |

**Returns:**
T - निर्दिष्ट अनुक्रमांक पर तत्व।
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


निर्धारित करता है कि संग्रह केवल‑पढ़ने योग्य है या नहीं।

**Returns:**
boolean - यदि संग्रह केवल‑पढ़ने योग्य है तो true; अन्यथा false।
### iterator() {#iterator--}
```
public final Iterator<T> iterator()
```


इस संग्रह के लिए एक एन्यूमरेटर लौटाता है।

**Returns:**
java.util.Iterator<T> - इस संग्रह के लिए एक इटेरेटर।
### remove(int index) {#remove-int-}
```
public final T remove(int index)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | \{@inheritDoc\} |

**Returns:**
T - {@inheritDoc}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
बूलियन - \{@inheritDoc\}
### set(int index, T value) {#set-int-T-}
```
public final T set(int index, T value)
```


निर्दिष्ट अनुक्रमांक पर तत्व लौटाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| सूचकांक | int | प्राप्त करने वाले तत्व का शून्य-आधारित अनुक्रमांक। |
| मान | T |  |

**Returns:**
T - निर्दिष्ट अनुक्रमांक पर तत्व।
### size() {#size--}
```
public final int size()
```


ऑब्जेक्ट में सम्मिलित वस्तुओं की संख्या प्राप्त करता है।

**Returns:**
int - ऑब्जेक्ट में सम्मिलित वस्तुओं की संख्या।
### toList() {#toList--}
```
public final List<T> toList()
```


संग्रह को वस्तुओं की सूची में परिवर्तित करता है।

**Returns:**
java.util.List<T> - वस्तुओं की सामान्य सूची।
