---
title: "ReadOnlyCollectionBase"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een alleen-lezen collectie van objecten voor."
type: docs
weight: 238
url: /nl/java/com.aspose.tasks/readonlycollectionbase/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public abstract class ReadOnlyCollectionBase<T> extends AbstractList<T>
```

Stelt een alleen-lezen collectie van objecten voor.

T : Type van verzamelingselementen.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [add(T item)](#add-T-) | Dit is de stub‑implementatie van de Add‑methode van ICollection, die alleen UnsupportedOperationException gooit. |
| [add(int index, T element)](#add-int-T-) | \{@inheritDoc\} |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | Retourneert het element op de opgegeven index. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Bepaalt of de collectie alleen‑lezen is. |
| [iterator()](#iterator--) | Retourneert een enumerator voor deze collectie. |
| [remove(int index)](#remove-int-) | \{@inheritDoc\} |
| [remove(Object o)](#remove-java.lang.Object-) | \{@inheritDoc\} |
| [set(int index, T value)](#set-int-T-) | Retourneert het element op de opgegeven index. |
| [size()](#size--) | Haalt het aantal objecten op dat in het object is opgenomen. |
| [toList()](#toList--) | Converteert de collectie naar een lijst van objecten. |
### add(T item) {#add-T-}
```
public final boolean add(T item)
```


Dit is de stub‑implementatie van de Add‑methode van ICollection, die alleen UnsupportedOperationException gooit.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | T | Het toe te voegen item. |

**Returns:**
boolean
### add(int index, T element) {#add-int-T-}
```
public final void add(int index, T element)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |
| element | T | \{@inheritDoc\} |

### clear() {#clear--}
```
public final void clear()
```




### contains(Object o) {#contains-java.lang.Object-}
```
public final boolean contains(Object o)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### get(int index) {#get-int-}
```
public final T get(int index)
```


Retourneert het element op de opgegeven index.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | De nulgebaseerde index van het element om op te halen. |

**Returns:**
T - het element op de opgegeven index.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Bepaalt of de collectie alleen‑lezen is.

**Returns:**
boolean - true als de collectie alleen‑lezen is; anders false.
### iterator() {#iterator--}
```
public final Iterator<T> iterator()
```


Retourneert een enumerator voor deze collectie.

**Returns:**
java.util.Iterator<T> - Een enumerator voor deze collectie.
### remove(int index) {#remove-int-}
```
public final T remove(int index)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
T - {@inheritDoc}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### set(int index, T value) {#set-int-T-}
```
public final T set(int index, T value)
```


Retourneert het element op de opgegeven index.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | De nulgebaseerde index van het element om op te halen. |
| waarde | T |  |

**Returns:**
T - het element op de opgegeven index.
### size() {#size--}
```
public final int size()
```


Haalt het aantal objecten op dat in het object is opgenomen.

**Returns:**
int - het aantal objecten dat in het object is opgenomen.
### toList() {#toList--}
```
public final List<T> toList()
```


Converteert de collectie naar een lijst van objecten.

**Returns:**
java.util.List<T> - Generieke lijst van objecten.
