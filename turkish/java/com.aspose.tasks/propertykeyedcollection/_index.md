---
title: "PropertyKeyedCollection"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Özellik koleksiyonunun temel sınıfı."
type: docs
weight: 231
url: /tr/java/com.aspose.tasks/propertykeyedcollection/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.PropertyCollection

**All Implemented Interfaces:**
java.util.Collection
```
public abstract class PropertyKeyedCollection<T> extends PropertyCollection<T> implements Collection<T>
```

Özellik koleksiyonunun temel sınıfı.

T : özelliğin tipi.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [&lt;T1&gt;toArray(T1[] a)](#-T1-toArray-T1---) | \{@inheritDoc\} |
| [add(T item)](#add-T-) | Yeni bir özel özellik oluşturur. |
| [addAll(Collection&lt;? extends T&gt; c)](#addAll-java.util.Collection---extends-T--) | \{@inheritDoc\} |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Object item)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [contains(String name)](#contains-java.lang.String-) | Aspose.Tasks.Properties.PropertyCollection<T>'nin belirtilen ada sahip bir özelliği içerip içermediğini belirler. |
| [containsAll(Collection&lt;?&gt; c)](#containsAll-java.util.Collection----) | \{@inheritDoc\} |
| [getNames()](#getNames--) | Tüm özellik adlarının koleksiyonunu alır. |
| [get_Item(String name)](#get-Item-java.lang.String-) | Belirtilen anahtarla ilişkili Özelliği alır. |
| [isEmpty()](#isEmpty--) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Bu koleksiyonun salt okunur olup olmadığını gösteren bir değeri alır; aksi takdirde false. |
| [remove(Object item)](#remove-java.lang.Object-) | \{@inheritDoc\} |
| [removeAll(Collection&lt;?&gt; c)](#removeAll-java.util.Collection----) | \{@inheritDoc\} |
| [retainAll(Collection&lt;?&gt; c)](#retainAll-java.util.Collection----) | \{@inheritDoc\} |
| [size()](#size--) | Koleksiyondaki özellik sayısını alır. |
| [toArray()](#toArray--) | \{@inheritDoc\} |
### &lt;T1&gt;toArray(T1[] a) {#-T1-toArray-T1---}
```
public T1[] <T1>toArray(T1[] a)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| a | T1[] | \{@inheritDoc\} |

**Returns:**
T1[] - \{@inheritDoc\}
### add(T item) {#add-T-}
```
public final boolean add(T item)
```


Yeni bir özel özellik oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| öğe | T | Eklenecek özellik. |

**Returns:**
boolean
### addAll(Collection&lt;? extends T&gt; c) {#addAll-java.util.Collection---extends-T--}
```
public boolean addAll(Collection<? extends T> c)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| c | java.util.Collection<? extends T> | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### clear() {#clear--}
```
public void clear()
```




### contains(Object item) {#contains-java.lang.Object-}
```
public final boolean contains(Object item)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| öğe | java.lang.Object |  |

**Returns:**
boolean
### contains(String name) {#contains-java.lang.String-}
```
public final boolean contains(String name)
```


Aspose.Tasks.Properties.PropertyCollection<T>'nin belirtilen ada sahip bir özelliği içerip içermediğini belirler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | java.lang.String | Bir özelliğin adı |

**Returns:**
boolean - Aspose.Tasks.Properties.PropertyCollection<T> belirtilen ada sahip bir özelliği içeriyorsa true; aksi takdirde false.
### containsAll(Collection&lt;?&gt; c) {#containsAll-java.util.Collection----}
```
public boolean containsAll(Collection<?> c)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| c | java.util.Collection<?> | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### getNames() {#getNames--}
```
public final Collection<String> getNames()
```


Tüm özellik adlarının koleksiyonunu alır.

**Returns:**
java.util.Collection<java.lang.String> - tüm özellik adlarının koleksiyonu.
### get_Item(String name) {#get-Item-java.lang.String-}
```
public final T get_Item(String name)
```


Belirtilen anahtarla ilişkili Özelliği alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | java.lang.String | Alınacak Özelliğin adı. |

**Returns:**
T - Belirtilen adla ilişkili Özellik.
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```




**Returns:**
boolean - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


Bu koleksiyonun salt okunur olup olmadığını gösteren bir değeri alır; aksi takdirde false.

**Returns:**
boolean - bu koleksiyonun yalnızca okunur olup olmadığını gösteren bir değer; aksi takdirde false.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| öğe | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### removeAll(Collection&lt;?&gt; c) {#removeAll-java.util.Collection----}
```
public boolean removeAll(Collection<?> c)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| c | java.util.Collection<?> | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### retainAll(Collection&lt;?&gt; c) {#retainAll-java.util.Collection----}
```
public boolean retainAll(Collection<?> c)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| c | java.util.Collection<?> | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### size() {#size--}
```
public final int size()
```


Koleksiyondaki özellik sayısını alır.

**Returns:**
int - koleksiyondaki özellik sayısı.
### toArray() {#toArray--}
```
public Object[] toArray()
```




**Returns:**
java.lang.Object[] - \{@inheritDoc\}
