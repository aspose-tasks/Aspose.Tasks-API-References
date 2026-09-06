---
title: "FilterCollection"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Contiene una lista de objetos."
type: docs
weight: 92
url: /es/java/com.aspose.tasks/filtercollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class FilterCollection extends AbstractCollection<Filter>
```

Contiene una lista de objetos [Filter](../../com.aspose.tasks/filter). Implementa la interfaz ICollection&lt;Filter&gt;.
## Métodos

| Método | Descripción |
| --- | --- |
| [add(Filter item)](#add-com.aspose.tasks.Filter-) |  |
| [clear()](#clear--) | Elimina todos los elementos de esta colección (operación opcional). |
| [contains(Filter item)](#contains-com.aspose.tasks.Filter-) | Devuelve true si esta colección contiene el elemento especificado. |
| [copyTo(Filter[] array, int arrayIndex)](#copyTo-com.aspose.tasks.Filter---int-) | Copia los elementos del array especificado a esta colección comenzando desde el índice especificado. |
| [iterator()](#iterator--) | Devuelve un iterador sobre los elementos contenidos en esta colección. |
| [remove(Filter item)](#remove-com.aspose.tasks.Filter-) | Elimina el elemento especificado de esta colección. |
| [size()](#size--) | Obtiene el número de elementos contenidos en esta colección. |
| [toList()](#toList--) | Convierte una colección de filtros en una lista de objetos `Filter`. |
### add(Filter item) {#add-com.aspose.tasks.Filter-}
```
public boolean add(Filter item)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) |  |

**Returns:**
boolean
### clear() {#clear--}
```
public void clear()
```


Elimina todos los elementos de esta colección (operación opcional).

### contains(Filter item) {#contains-com.aspose.tasks.Filter-}
```
public final boolean contains(Filter item)
```


Devuelve true si esta colección contiene el elemento especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) | el elemento especificado. |

**Returns:**
boolean - true si la colección contiene el elemento especificado.
### copyTo(Filter[] array, int arrayIndex) {#copyTo-com.aspose.tasks.Filter---int-}
```
public final void copyTo(Filter[] array, int arrayIndex)
```


Copia los elementos del array especificado a esta colección comenzando desde el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| array | [Filter\[\]](../../com.aspose.tasks/filter) | el array unidimensional especificado al que copiar los elementos |
| arrayIndex | int | el índice basado en cero del array especificado en el que comienza la copia. |

### iterator() {#iterator--}
```
public Iterator<Filter> iterator()
```


Devuelve un iterador sobre los elementos contenidos en esta colección.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Filter&gt; - iterador de colección.
### remove(Filter item) {#remove-com.aspose.tasks.Filter-}
```
public final boolean remove(Filter item)
```


Elimina el elemento especificado de esta colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) | el elemento especificado. |

**Returns:**
boolean - true si la operación fue exitosa.
### size() {#size--}
```
public final int size()
```


Obtiene el número de elementos contenidos en esta colección.

**Returns:**
int - el número de elementos contenidos en esta colección.
### toList() {#toList--}
```
public List<Filter> toList()
```


Convierte una colección de filtros en una lista de objetos `Filter`.

**Returns:**
java.util.List&lt;com.aspose.tasks.Filter&gt; - Lista genérica de objetos `Filter`.
