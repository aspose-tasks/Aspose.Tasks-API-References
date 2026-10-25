---
title: "ReadOnlyCollectionBase"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa una colección de solo lectura de objetos."
type: docs
weight: 238
url: /es/java/com.aspose.tasks/readonlycollectionbase/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public abstract class ReadOnlyCollectionBase<T> extends AbstractList<T>
```

Representa una colección de solo lectura de objetos.

T : Tipo de elementos de la colección.
## Métodos

| Método | Descripción |
| --- | --- |
| [add(T item)](#add-T-) | Esta es la implementación de sustituto del método Add de ICollection, que solo lanza UnsupportedOperationException |
| [add(int index, T element)](#add-int-T-) | \{@inheritDoc\} |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | Devuelve el elemento en el índice especificado. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Determina si la colección es de solo lectura. |
| [iterator()](#iterator--) | Devuelve un enumerador para esta colección. |
| [remove(int index)](#remove-int-) | \{@inheritDoc\} |
| [remove(Object o)](#remove-java.lang.Object-) | \{@inheritDoc\} |
| [set(int index, T value)](#set-int-T-) | Devuelve el elemento en el índice especificado. |
| [size()](#size--) | Obtiene el número de objetos contenidos en el objeto. |
| [toList()](#toList--) | Convierte la colección en una lista de objetos. |
### add(T item) {#add-T-}
```
public final boolean add(T item)
```


Esta es la implementación de sustituto del método Add de ICollection, que solo lanza UnsupportedOperationException

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| elemento | T | El elemento a añadir. |

**Returns:**
boolean
### add(int index, T element) {#add-int-T-}
```
public final void add(int index, T element)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | \{@inheritDoc\} |
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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### get(int index) {#get-int-}
```
public final T get(int index)
```


Devuelve el elemento en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice basado en cero del elemento a obtener. |

**Returns:**
T - el elemento en el índice especificado.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Determina si la colección es de solo lectura.

**Returns:**
boolean - true si la colección es de solo lectura; false en caso contrario.
### iterator() {#iterator--}
```
public final Iterator<T> iterator()
```


Devuelve un enumerador para esta colección.

**Returns:**
java.util.Iterator<T> - Un enumerador para esta colección.
### remove(int index) {#remove-int-}
```
public final T remove(int index)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | \{@inheritDoc\} |

**Returns:**
T - {@inheritDoc}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### set(int index, T value) {#set-int-T-}
```
public final T set(int index, T value)
```


Devuelve el elemento en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice basado en cero del elemento a obtener. |
| valor | T |  |

**Returns:**
T - el elemento en el índice especificado.
### size() {#size--}
```
public final int size()
```


Obtiene el número de objetos contenidos en el objeto.

**Returns:**
int - el número de objetos contenidos en el objeto.
### toList() {#toList--}
```
public final List<T> toList()
```


Convierte la colección en una lista de objetos.

**Returns:**
java.util.List<T> - Lista genérica de objetos.
