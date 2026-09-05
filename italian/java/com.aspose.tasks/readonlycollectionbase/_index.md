---
title: "ReadOnlyCollectionBase"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta una raccolta di oggetti in sola lettura."
type: docs
weight: 238
url: /it/java/com.aspose.tasks/readonlycollectionbase/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public abstract class ReadOnlyCollectionBase<T> extends AbstractList<T>
```

Rappresenta una raccolta di oggetti in sola lettura.

T : Tipo degli elementi della collezione.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(T item)](#add-T-) | Questa è l'implementazione stub del metodo Add di ICollection, che lancia solo UnsupportedOperationException |
| [add(int index, T element)](#add-int-T-) | \{@inheritDoc\} |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | Restituisce l'elemento all'indice specificato. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Determina se la collezione è di sola lettura. |
| [iterator()](#iterator--) | Restituisce un enumeratore per questa collezione. |
| [remove(int index)](#remove-int-) | \{@inheritDoc\} |
| [remove(Object o)](#remove-java.lang.Object-) | \{@inheritDoc\} |
| [set(int index, T value)](#set-int-T-) | Restituisce l'elemento all'indice specificato. |
| [size()](#size--) | Ottiene il numero di oggetti contenuti nell'oggetto. |
| [toList()](#toList--) | Converte la collezione in un elenco di oggetti. |
### add(T item) {#add-T-}
```
public final boolean add(T item)
```


Questa è l'implementazione stub del metodo Add di ICollection, che lancia solo UnsupportedOperationException

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| elemento | T | L'elemento da aggiungere. |

**Returns:**
boolean
### add(int index, T element) {#add-int-T-}
```
public final void add(int index, T element)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |
| elemento | T | \{@inheritDoc\} |

### clear() {#clear--}
```
public final void clear()
```




### contains(Object o) {#contains-java.lang.Object-}
```
public final boolean contains(Object o)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### get(int index) {#get-int-}
```
public final T get(int index)
```


Restituisce l'elemento all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | L'indice basato su zero dell'elemento da ottenere. |

**Returns:**
T - l'elemento all'indice specificato.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Determina se la collezione è di sola lettura.

**Returns:**
boolean - true se la collezione è di sola lettura; false altrimenti.
### iterator() {#iterator--}
```
public final Iterator<T> iterator()
```


Restituisce un enumeratore per questa collezione.

**Returns:**
java.util.Iterator<T> - Un enumeratore per questa collezione.
### remove(int index) {#remove-int-}
```
public final T remove(int index)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
T - {@inheritDoc}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### set(int index, T value) {#set-int-T-}
```
public final T set(int index, T value)
```


Restituisce l'elemento all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | L'indice basato su zero dell'elemento da ottenere. |
| valore | T |  |

**Returns:**
T - l'elemento all'indice specificato.
### size() {#size--}
```
public final int size()
```


Ottiene il numero di oggetti contenuti nell'oggetto.

**Returns:**
int - il numero di oggetti contenuti nell'oggetto.
### toList() {#toList--}
```
public final List<T> toList()
```


Converte la collezione in un elenco di oggetti.

**Returns:**
java.util.List<T> - Elenco generico di oggetti.
