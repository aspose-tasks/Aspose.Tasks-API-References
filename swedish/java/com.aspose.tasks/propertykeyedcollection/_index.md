---
title: "PropertyKeyedCollection"
second_title: "Aspose.Tasks for Java API-referens"
description: "En basklass för en samling av egenskaper."
type: docs
weight: 231
url: /sv/java/com.aspose.tasks/propertykeyedcollection/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.PropertyCollection

**All Implemented Interfaces:**
java.util.Collection
```
public abstract class PropertyKeyedCollection<T> extends PropertyCollection<T> implements Collection<T>
```

En basklass för en samling av egenskaper.

T : typen av egenskap.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [&lt;T1&gt;toArray(T1[] a)](#-T1-toArray-T1---) | \{@inheritDoc\} |
| [add(T item)](#add-T-) | Skapar en ny anpassad egenskap. |
| [addAll(Collection&lt;? extends T&gt; c)](#addAll-java.util.Collection---extends-T--) | \{@inheritDoc\} |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Object item)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [contains(String name)](#contains-java.lang.String-) | Bestämmer om Aspose.Tasks.Properties.PropertyCollection&lt;T&gt; innehåller en egenskap med det angivna namnet. |
| [containsAll(Collection&lt;?&gt; c)](#containsAll-java.util.Collection----) | \{@inheritDoc\} |
| [getNames()](#getNames--) | Hämtar samlingen av alla egenskapsnamn. |
| [get_Item(String name)](#get-Item-java.lang.String-) | Hämtar Property som är associerad med den angivna nyckeln. |
| [isEmpty()](#isEmpty--) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Hämtar ett värde som anger om den här samlingen är skrivskyddad; annars falskt. |
| [remove(Object item)](#remove-java.lang.Object-) | \{@inheritDoc\} |
| [removeAll(Collection&lt;?&gt; c)](#removeAll-java.util.Collection----) | \{@inheritDoc\} |
| [retainAll(Collection&lt;?&gt; c)](#retainAll-java.util.Collection----) | \{@inheritDoc\} |
| [size()](#size--) | Hämtar antalet egenskaper i samlingen. |
| [toArray()](#toArray--) | \{@inheritDoc\} |
### &lt;T1&gt;toArray(T1[] a) {#-T1-toArray-T1---}
```
public T1[] <T1>toArray(T1[] a)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| a | T1[] | \{@inheritDoc\} |

**Returns:**
T1[] - \{@inheritDoc\}
### add(T item) {#add-T-}
```
public final boolean add(T item)
```


Skapar en ny anpassad egenskap.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| objekt | T | Egenskapen att lägga till. |

**Returns:**
boolean
### addAll(Collection&lt;? extends T&gt; c) {#addAll-java.util.Collection---extends-T--}
```
public boolean addAll(Collection<? extends T> c)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| c | java.util.Collection&lt;? extends T&gt; | \{@inheritDoc\} |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| objekt | java.lang.Object |  |

**Returns:**
boolean
### contains(String name) {#contains-java.lang.String-}
```
public final boolean contains(String name)
```


Bestämmer om Aspose.Tasks.Properties.PropertyCollection&lt;T&gt; innehåller en egenskap med det angivna namnet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Namnet på en egenskap |

**Returns:**
boolean - true om Aspose.Tasks.Properties.PropertyCollection&lt;T&gt; innehåller en egenskap med det angivna namnet; annars false.
### containsAll(Collection&lt;?&gt; c) {#containsAll-java.util.Collection----}
```
public boolean containsAll(Collection<?> c)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| c | java.util.Collection&lt;?&gt; | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### getNames() {#getNames--}
```
public final Collection<String> getNames()
```


Hämtar samlingen av alla egenskapsnamn.

**Returns:**
java.util.Collection&lt;java.lang.String&gt; - samlingen av alla egenskapsnamn.
### get_Item(String name) {#get-Item-java.lang.String-}
```
public final T get_Item(String name)
```


Hämtar Property som är associerad med den angivna nyckeln.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Namnet på Property som ska hämtas. |

**Returns:**
T - Property som är associerad med det angivna namnet.
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


Hämtar ett värde som anger om den här samlingen är skrivskyddad; annars falskt.

**Returns:**
boolean - ett värde som indikerar om denna samling är skrivskyddad; annars falskt.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| objekt | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### removeAll(Collection&lt;?&gt; c) {#removeAll-java.util.Collection----}
```
public boolean removeAll(Collection<?> c)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| c | java.util.Collection&lt;?&gt; | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### retainAll(Collection&lt;?&gt; c) {#retainAll-java.util.Collection----}
```
public boolean retainAll(Collection<?> c)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| c | java.util.Collection&lt;?&gt; | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### size() {#size--}
```
public final int size()
```


Hämtar antalet egenskaper i samlingen.

**Returns:**
int - antalet egenskaper i samlingen.
### toArray() {#toArray--}
```
public Object[] toArray()
```




**Returns:**
java.lang.Object[] - \{@inheritDoc\}
