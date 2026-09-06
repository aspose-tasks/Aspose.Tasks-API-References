---
title: "ReadOnlyCollectionBase"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en skrivskyddad samling av objekt."
type: docs
weight: 238
url: /sv/java/com.aspose.tasks/readonlycollectionbase/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public abstract class ReadOnlyCollectionBase<T> extends AbstractList<T>
```

Representerar en skrivskyddad samling av objekt.

T : Typ av samlingsobjekt.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(T item)](#add-T-) | Detta är stub-implementationen av ICollection:s Add‑metod, som endast kastar UnsupportedOperationException. |
| [add(int index, T element)](#add-int-T-) | \{@inheritDoc\} |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | Returnerar elementet på det angivna indexet. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Avgör om samlingen är skrivskyddad. |
| [iterator()](#iterator--) | Returnerar en enumerator för denna samling. |
| [remove(int index)](#remove-int-) | \{@inheritDoc\} |
| [remove(Object o)](#remove-java.lang.Object-) | \{@inheritDoc\} |
| [set(int index, T value)](#set-int-T-) | Returnerar elementet på det angivna indexet. |
| [size()](#size--) | Hämtar antalet objekt som finns i objektet. |
| [toList()](#toList--) | Konverterar samlingen till en lista med objekt. |
### add(T item) {#add-T-}
```
public final boolean add(T item)
```


Detta är stub-implementationen av ICollection:s Add‑metod, som endast kastar UnsupportedOperationException.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| objekt | T | Objektet att lägga till. |

**Returns:**
boolean
### add(int index, T element) {#add-int-T-}
```
public final void add(int index, T element)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### get(int index) {#get-int-}
```
public final T get(int index)
```


Returnerar elementet på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Det nollbaserade indexet för elementet att hämta. |

**Returns:**
T – elementet på det angivna indexet.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int – \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Avgör om samlingen är skrivskyddad.

**Returns:**
boolean – true om samlingen är skrivskyddad; false annars.
### iterator() {#iterator--}
```
public final Iterator<T> iterator()
```


Returnerar en enumerator för denna samling.

**Returns:**
java.util.Iterator<T> – En enumerator för denna samling.
### remove(int index) {#remove-int-}
```
public final T remove(int index)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
T - {@inheritDoc}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### set(int index, T value) {#set-int-T-}
```
public final T set(int index, T value)
```


Returnerar elementet på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Det nollbaserade indexet för elementet att hämta. |
| värde | T |  |

**Returns:**
T – elementet på det angivna indexet.
### size() {#size--}
```
public final int size()
```


Hämtar antalet objekt som finns i objektet.

**Returns:**
int – antalet objekt som finns i objektet.
### toList() {#toList--}
```
public final List<T> toList()
```


Konverterar samlingen till en lista med objekt.

**Returns:**
java.util.List<T> – Generisk lista med objekt.
