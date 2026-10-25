---
title: "ReadOnlyCollectionBase"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt eine schreibgeschützte Sammlung von Objekten dar."
type: docs
weight: 238
url: /de/java/com.aspose.tasks/readonlycollectionbase/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public abstract class ReadOnlyCollectionBase<T> extends AbstractList<T>
```

Stellt eine schreibgeschützte Sammlung von Objekten dar.

T : Typ der Sammlungselemente.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(T item)](#add-T-) | Dies ist die Stub‑Implementierung der Add‑Methode von ICollection, die nur UnsupportedOperationException wirft. |
| [add(int index, T element)](#add-int-T-) | \{@inheritDoc\} |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | Gibt das Element am angegebenen Index zurück. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Bestimmt, ob die Sammlung schreibgeschützt ist. |
| [iterator()](#iterator--) | Gibt einen Enumerator für diese Sammlung zurück. |
| [remove(int index)](#remove-int-) | \{@inheritDoc\} |
| [remove(Object o)](#remove-java.lang.Object-) | \{@inheritDoc\} |
| [set(int index, T value)](#set-int-T-) | Gibt das Element am angegebenen Index zurück. |
| [size()](#size--) | Gibt die Anzahl der im Objekt enthaltenen Objekte zurück. |
| [toList()](#toList--) | Konvertiert die Sammlung in eine Liste von Objekten. |
### add(T item) {#add-T-}
```
public final boolean add(T item)
```


Dies ist die Stub‑Implementierung der Add‑Methode von ICollection, die nur UnsupportedOperationException wirft.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Element | T | Das hinzuzufügende Element. |

**Returns:**
boolean
### add(int index, T element) {#add-int-T-}
```
public final void add(int index, T element)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | \{@inheritDoc\} |
| Element | T | \{@inheritDoc\} |

### clear() {#clear--}
```
public final void clear()
```




### contains(Object o) {#contains-java.lang.Object-}
```
public final boolean contains(Object o)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \\{@inheritDoc\\}
### get(int index) {#get-int-}
```
public final T get(int index)
```


Gibt das Element am angegebenen Index zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der nullbasierte Index des abzurufenden Elements. |

**Returns:**
T - das Element am angegebenen Index.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Bestimmt, ob die Sammlung schreibgeschützt ist.

**Returns:**
boolean - true, wenn die Sammlung schreibgeschützt ist; sonst false.
### iterator() {#iterator--}
```
public final Iterator<T> iterator()
```


Gibt einen Enumerator für diese Sammlung zurück.

**Returns:**
java.util.Iterator&lt;T&gt; - Ein Enumerator für diese Sammlung.
### remove(int index) {#remove-int-}
```
public final T remove(int index)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | \{@inheritDoc\} |

**Returns:**
T - \{@inheritDoc\}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \\{@inheritDoc\\}
### set(int index, T value) {#set-int-T-}
```
public final T set(int index, T value)
```


Gibt das Element am angegebenen Index zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der nullbasierte Index des abzurufenden Elements. |
| Wert | T |  |

**Returns:**
T - das Element am angegebenen Index.
### size() {#size--}
```
public final int size()
```


Gibt die Anzahl der im Objekt enthaltenen Objekte zurück.

**Returns:**
int - die Anzahl der im Objekt enthaltenen Objekte.
### toList() {#toList--}
```
public final List<T> toList()
```


Konvertiert die Sammlung in eine Liste von Objekten.

**Returns:**
java.util.List&lt;T&gt; - Generische Liste von Objekten.
