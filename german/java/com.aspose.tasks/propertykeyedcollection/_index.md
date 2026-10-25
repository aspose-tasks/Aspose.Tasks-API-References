---
title: "PropertyKeyedCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "Eine Basisklasse einer Sammlung von Eigenschaften."
type: docs
weight: 231
url: /de/java/com.aspose.tasks/propertykeyedcollection/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.PropertyCollection

**All Implemented Interfaces:**
java.util.Collection
```
public abstract class PropertyKeyedCollection<T> extends PropertyCollection<T> implements Collection<T>
```

Eine Basisklasse einer Sammlung von Eigenschaften.

T : der Typ der Eigenschaft.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [&lt;T1&gt;toArray(T1[] a)](#-T1-toArray-T1---) | \{@inheritDoc\} |
| [add(T item)](#add-T-) | Erstellt eine neue benutzerdefinierte Eigenschaft. |
| [addAll(Collection&lt;? extends T&gt; c)](#addAll-java.util.Collection---extends-T--) | \{@inheritDoc\} |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Object item)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [contains(String name)](#contains-java.lang.String-) | Bestimmt, ob die Aspose.Tasks.Properties.PropertyCollection&lt;T&gt; eine Eigenschaft mit dem angegebenen Namen enthält. |
| [containsAll(Collection&lt;?&gt; c)](#containsAll-java.util.Collection----) | \{@inheritDoc\} |
| [getNames()](#getNames--) | Ruft die Sammlung aller Eigenschaftsnamen ab. |
| [get_Item(String name)](#get-Item-java.lang.String-) | Ruft die Property ab, die dem angegebenen Schlüssel zugeordnet ist. |
| [isEmpty()](#isEmpty--) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Ruft einen Wert ab, der angibt, ob diese Sammlung schreibgeschützt ist; andernfalls false. |
| [remove(Object item)](#remove-java.lang.Object-) | \{@inheritDoc\} |
| [removeAll(Collection&lt;?&gt; c)](#removeAll-java.util.Collection----) | \{@inheritDoc\} |
| [retainAll(Collection&lt;?&gt; c)](#retainAll-java.util.Collection----) | \{@inheritDoc\} |
| [size()](#size--) | Ruft die Anzahl der Eigenschaften in der Sammlung ab. |
| [toArray()](#toArray--) | \{@inheritDoc\} |
### &lt;T1&gt;toArray(T1[] a) {#-T1-toArray-T1---}
```
public T1[] <T1>toArray(T1[] a)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| a | T1[] | \{@inheritDoc\} |

**Returns:**
T1[] - \{@inheritDoc\}
### add(T item) {#add-T-}
```
public final boolean add(T item)
```


Erstellt eine neue benutzerdefinierte Eigenschaft.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Element | T | Die hinzuzufügende Eigenschaft. |

**Returns:**
boolean
### addAll(Collection&lt;? extends T&gt; c) {#addAll-java.util.Collection---extends-T--}
```
public boolean addAll(Collection<? extends T> c)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| c | java.util.Collection&lt;? extends T&gt; | \{@inheritDoc\} |

**Returns:**
boolean - \\{@inheritDoc\\}
### clear() {#clear--}
```
public void clear()
```




### contains(Object item) {#contains-java.lang.Object-}
```
public final boolean contains(Object item)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Element | java.lang.Object |  |

**Returns:**
boolean
### contains(String name) {#contains-java.lang.String-}
```
public final boolean contains(String name)
```


Bestimmt, ob die Aspose.Tasks.Properties.PropertyCollection&lt;T&gt; eine Eigenschaft mit dem angegebenen Namen enthält.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | java.lang.String | Der Name einer Eigenschaft |

**Returns:**
boolean - true, wenn die Aspose.Tasks.Properties.PropertyCollection&lt;T&gt; eine Eigenschaft mit dem angegebenen Namen enthält; andernfalls false.
### containsAll(Collection&lt;?&gt; c) {#containsAll-java.util.Collection----}
```
public boolean containsAll(Collection<?> c)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| c | java.util.Collection&lt;?&gt; | \{@inheritDoc\} |

**Returns:**
boolean - \\{@inheritDoc\\}
### getNames() {#getNames--}
```
public final Collection<String> getNames()
```


Ruft die Sammlung aller Eigenschaftsnamen ab.

**Returns:**
java.util.Collection&lt;java.lang.String&gt; - die Sammlung aller Eigenschaftsnamen.
### get_Item(String name) {#get-Item-java.lang.String-}
```
public final T get_Item(String name)
```


Ruft die Property ab, die dem angegebenen Schlüssel zugeordnet ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | java.lang.String | Der Name der Property, die abgerufen werden soll. |

**Returns:**
T - Die Property, die mit dem angegebenen Namen verknüpft ist.
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```




**Returns:**
boolean - \\{@inheritDoc\\}
### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


Ruft einen Wert ab, der angibt, ob diese Sammlung schreibgeschützt ist; andernfalls false.

**Returns:**
boolean - ein Wert, der angibt, ob diese Sammlung schreibgeschützt ist; andernfalls false.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Element | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \\{@inheritDoc\\}
### removeAll(Collection&lt;?&gt; c) {#removeAll-java.util.Collection----}
```
public boolean removeAll(Collection<?> c)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| c | java.util.Collection&lt;?&gt; | \{@inheritDoc\} |

**Returns:**
boolean - \\{@inheritDoc\\}
### retainAll(Collection&lt;?&gt; c) {#retainAll-java.util.Collection----}
```
public boolean retainAll(Collection<?> c)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| c | java.util.Collection&lt;?&gt; | \{@inheritDoc\} |

**Returns:**
boolean - \\{@inheritDoc\\}
### size() {#size--}
```
public final int size()
```


Ruft die Anzahl der Eigenschaften in der Sammlung ab.

**Returns:**
int - die Anzahl der Eigenschaften in der Sammlung.
### toArray() {#toArray--}
```
public Object[] toArray()
```




**Returns:**
java.lang.Object[] - \{@inheritDoc\}
