---
title: "PropertyKeyedCollection"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Een basisklasse van een verzameling eigenschappen."
type: docs
weight: 231
url: /nl/java/com.aspose.tasks/propertykeyedcollection/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.PropertyCollection

**All Implemented Interfaces:**
java.util.Collection
```
public abstract class PropertyKeyedCollection<T> extends PropertyCollection<T> implements Collection<T>
```

Een basisklasse van een verzameling eigenschappen.

T : het type van de eigenschap.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [&lt;T1&gt;toArray(T1[] a)](#-T1-toArray-T1---) | \{@inheritDoc\} |
| [add(T item)](#add-T-) | Maakt een nieuwe aangepaste eigenschap aan. |
| [addAll(Collection&lt;? extends T&gt; c)](#addAll-java.util.Collection---extends-T--) | \{@inheritDoc\} |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Object item)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [contains(String name)](#contains-java.lang.String-) | Bepaalt of de Aspose.Tasks.Properties.PropertyCollection<T> een eigenschap bevat met de opgegeven naam. |
| [containsAll(Collection&lt;?&gt; c)](#containsAll-java.util.Collection----) | \{@inheritDoc\} |
| [getNames()](#getNames--) | Haalt de collectie van alle eigenschapsnamen op. |
| [get_Item(String name)](#get-Item-java.lang.String-) | Haalt de Property op die geassocieerd is met de opgegeven sleutel. |
| [isEmpty()](#isEmpty--) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Haalt een waarde op die aangeeft of deze collectie alleen-lezen is; anders false. |
| [remove(Object item)](#remove-java.lang.Object-) | \{@inheritDoc\} |
| [removeAll(Collection&lt;?&gt; c)](#removeAll-java.util.Collection----) | \{@inheritDoc\} |
| [retainAll(Collection&lt;?&gt; c)](#retainAll-java.util.Collection----) | \{@inheritDoc\} |
| [size()](#size--) | Haalt het aantal eigenschappen op in de collectie. |
| [toArray()](#toArray--) | \{@inheritDoc\} |
### &lt;T1&gt;toArray(T1[] a) {#-T1-toArray-T1---}
```
public T1[] <T1>toArray(T1[] a)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| een | T1[] | \{@inheritDoc\} |

**Returns:**
T1[] - \{@inheritDoc\}
### add(T item) {#add-T-}
```
public final boolean add(T item)
```


Maakt een nieuwe aangepaste eigenschap aan.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | T | De toe te voegen eigenschap. |

**Returns:**
boolean
### addAll(Collection&lt;? extends T&gt; c) {#addAll-java.util.Collection---extends-T--}
```
public boolean addAll(Collection<? extends T> c)
```




**Parameters:**
| Parameter | Type | Beschrijving |
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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | java.lang.Object |  |

**Returns:**
boolean
### contains(String name) {#contains-java.lang.String-}
```
public final boolean contains(String name)
```


Bepaalt of de Aspose.Tasks.Properties.PropertyCollection<T> een eigenschap bevat met de opgegeven naam.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | De naam van een eigenschap |

**Returns:**
boolean - true als de Aspose.Tasks.Properties.PropertyCollection<T> een eigenschap bevat met de opgegeven naam; anders false.
### containsAll(Collection&lt;?&gt; c) {#containsAll-java.util.Collection----}
```
public boolean containsAll(Collection<?> c)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| c | java.util.Collection<?> | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### getNames() {#getNames--}
```
public final Collection<String> getNames()
```


Haalt de collectie van alle eigenschapsnamen op.

**Returns:**
java.util.Collection<java.lang.String> - de collectie van alle eigenschapsnamen.
### get_Item(String name) {#get-Item-java.lang.String-}
```
public final T get_Item(String name)
```


Haalt de Property op die geassocieerd is met de opgegeven sleutel.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | De naam van de Property om op te halen. |

**Returns:**
T - De Property die geassocieerd is met de opgegeven naam.
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


Haalt een waarde op die aangeeft of deze collectie alleen-lezen is; anders false.

**Returns:**
boolean - een waarde die aangeeft of deze collectie alleen-lezen is; anders false.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### removeAll(Collection&lt;?&gt; c) {#removeAll-java.util.Collection----}
```
public boolean removeAll(Collection<?> c)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| c | java.util.Collection<?> | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### retainAll(Collection&lt;?&gt; c) {#retainAll-java.util.Collection----}
```
public boolean retainAll(Collection<?> c)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| c | java.util.Collection<?> | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### size() {#size--}
```
public final int size()
```


Haalt het aantal eigenschappen op in de collectie.

**Returns:**
int - het aantal eigenschappen in de collectie.
### toArray() {#toArray--}
```
public Object[] toArray()
```




**Returns:**
java.lang.Object[] - \{@inheritDoc\}
