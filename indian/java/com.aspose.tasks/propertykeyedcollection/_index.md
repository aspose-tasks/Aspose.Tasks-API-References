---
title: "PropertyKeyedCollection"
second_title: "Aspose.Tasks के लिए Java API Reference"
description: "प्रॉपर्टीज़ के संग्रह की बेस क्लास।"
type: docs
weight: 231
url: /hi/java/com.aspose.tasks/propertykeyedcollection/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.PropertyCollection

**All Implemented Interfaces:**
java.util.Collection
```
public abstract class PropertyKeyedCollection<T> extends PropertyCollection<T> implements Collection<T>
```

प्रॉपर्टीज़ के संग्रह की बेस क्लास।

T : प्रॉपर्टी का प्रकार।
## विधियाँ

| विधि | विवरण |
| --- | --- |
| [&lt;T1&gt;toArray(T1[] a)](#-T1-toArray-T1---) | \{@inheritDoc\} |
| [add(T item)](#add-T-) | एक नई कस्टम प्रॉपर्टी बनाता है। |
| [addAll(Collection&lt;? extends T&gt; c)](#addAll-java.util.Collection---extends-T--) | \{@inheritDoc\} |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Object item)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [contains(String name)](#contains-java.lang.String-) | निर्धारित करता है कि Aspose.Tasks.Properties.PropertyCollection<T> में निर्दिष्ट नाम वाली प्रॉपर्टी मौजूद है या नहीं। |
| [containsAll(Collection&lt;?&gt; c)](#containsAll-java.util.Collection----) | \{@inheritDoc\} |
| [getNames()](#getNames--) | सभी प्रॉपर्टी नामों का संग्रह प्राप्त करता है। |
| [get_Item(String name)](#get-Item-java.lang.String-) | निर्दिष्ट कुंजी से संबंधित प्रॉपर्टी प्राप्त करता है। |
| [isEmpty()](#isEmpty--) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | एक मान प्राप्त करता है जो दर्शाता है कि यह संग्रह केवल-पढ़ने योग्य है या नहीं; अन्यथा, false। |
| [remove(Object item)](#remove-java.lang.Object-) | \{@inheritDoc\} |
| [removeAll(Collection&lt;?&gt; c)](#removeAll-java.util.Collection----) | \{@inheritDoc\} |
| [retainAll(Collection&lt;?&gt; c)](#retainAll-java.util.Collection----) | \{@inheritDoc\} |
| [size()](#size--) | संग्रह में प्रॉपर्टियों की संख्या प्राप्त करता है। |
| [toArray()](#toArray--) | \{@inheritDoc\} |
### &lt;T1&gt;toArray(T1[] a) {#-T1-toArray-T1---}
```
public T1[] <T1>toArray(T1[] a)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| एक | T1[] | \{@inheritDoc\} |

**Returns:**
T1[] - \{@inheritDoc\}
### add(T item) {#add-T-}
```
public final boolean add(T item)
```


एक नई कस्टम प्रॉपर्टी बनाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| item | T | जोड़ने के लिए प्रॉपर्टी। |

**Returns:**
boolean
### addAll(Collection&lt;? extends T&gt; c) {#addAll-java.util.Collection---extends-T--}
```
public boolean addAll(Collection<? extends T> c)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| c | java.util.Collection<? extends T> | \{@inheritDoc\} |

**Returns:**
बूलियन - \{@inheritDoc\}
### clear() {#clear--}
```
public void clear()
```




### contains(Object item) {#contains-java.lang.Object-}
```
public final boolean contains(Object item)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| item | java.lang.Object |  |

**Returns:**
boolean
### contains(String name) {#contains-java.lang.String-}
```
public final boolean contains(String name)
```


निर्धारित करता है कि Aspose.Tasks.Properties.PropertyCollection<T> में निर्दिष्ट नाम वाली प्रॉपर्टी मौजूद है या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | java.lang.String | एक प्रॉपर्टी का नाम |

**Returns:**
boolean - true यदि Aspose.Tasks.Properties.PropertyCollection<T> में निर्दिष्ट नाम वाली प्रॉपर्टी मौजूद है; अन्यथा false।
### containsAll(Collection&lt;?&gt; c) {#containsAll-java.util.Collection----}
```
public boolean containsAll(Collection<?> c)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| c | java.util.Collection<?> | \{@inheritDoc\} |

**Returns:**
बूलियन - \{@inheritDoc\}
### getNames() {#getNames--}
```
public final Collection<String> getNames()
```


सभी प्रॉपर्टी नामों का संग्रह प्राप्त करता है।

**Returns:**
java.util.Collection<java.lang.String> - सभी प्रॉपर्टी नामों का संग्रह।
### get_Item(String name) {#get-Item-java.lang.String-}
```
public final T get_Item(String name)
```


निर्दिष्ट कुंजी से संबंधित प्रॉपर्टी प्राप्त करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | java.lang.String | प्राप्त करने के लिए प्रॉपर्टी का नाम। |

**Returns:**
T - निर्दिष्ट नाम से संबंधित प्रॉपर्टी।
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```




**Returns:**
बूलियन - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


एक मान प्राप्त करता है जो दर्शाता है कि यह संग्रह केवल-पढ़ने योग्य है या नहीं; अन्यथा, false।

**Returns:**
boolean - यह दर्शाने वाला मान कि यह संग्रह केवल-पढ़ने योग्य है; अन्यथा, false।
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| item | java.lang.Object | \{@inheritDoc\} |

**Returns:**
बूलियन - \{@inheritDoc\}
### removeAll(Collection&lt;?&gt; c) {#removeAll-java.util.Collection----}
```
public boolean removeAll(Collection<?> c)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| c | java.util.Collection<?> | \{@inheritDoc\} |

**Returns:**
बूलियन - \{@inheritDoc\}
### retainAll(Collection&lt;?&gt; c) {#retainAll-java.util.Collection----}
```
public boolean retainAll(Collection<?> c)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| c | java.util.Collection<?> | \{@inheritDoc\} |

**Returns:**
बूलियन - \{@inheritDoc\}
### size() {#size--}
```
public final int size()
```


संग्रह में प्रॉपर्टियों की संख्या प्राप्त करता है।

**Returns:**
int - संग्रह में प्रॉपर्टियों की संख्या।
### toArray() {#toArray--}
```
public Object[] toArray()
```




**Returns:**
java.lang.Object[] - \{@inheritDoc\}
