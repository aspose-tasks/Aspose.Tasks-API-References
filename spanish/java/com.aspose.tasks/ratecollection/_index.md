---
title: "RateCollection"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa una colección que contiene objetos."
type: docs
weight: 234
url: /es/java/com.aspose.tasks/ratecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractMap

**All Implemented Interfaces:**
java.lang.Iterable
```
public class RateCollection extends AbstractMap<Integer,RateByDateCollection> implements Iterable<Map.Entry<Integer,RateByDateCollection>>
```

Representa una colección que contiene objetos [Rate](../../com.aspose.tasks/rate).
## Métodos

| Método | Descripción |
| --- | --- |
| [add(Date ratesFrom)](#add-java.util.Date-) | Agrega una nueva instancia de [Rate](../../com.aspose.tasks/rate) a esta colección. |
| [add(Date ratesFrom, int type)](#add-java.util.Date-int-) | Agrega una nueva instancia de [Rate](../../com.aspose.tasks/rate) a esta colección. |
| [clear()](#clear--) | \{@inheritDoc\} |
| [entrySet()](#entrySet--) | (@inheritDoc\} |
| [get(Object key)](#get-java.lang.Object-) | (@inheritDoc\} |
| [getByRateType(int key)](#getByRateType-int-) | Devuelve el elemento en el índice especificado. |
| [getParentResource()](#getParentResource--) | Obtiene el objeto [Resource](../../com.aspose.tasks/resource) padre para esta colección. |
| [isReadOnly()](#isReadOnly--) | Obtiene un valor que indica si esta colección es de solo lectura. |
| [iterator()](#iterator--) | Devuelve un enumerador para esta colección. |
| [put(Integer key, RateByDateCollection value)](#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-) | (@inheritDoc\} |
| [remove(Rate item)](#remove-com.aspose.tasks.Rate-) | Elimina la instancia de Rate de esta colección. |
| [setByRateType(int key, RateByDateCollection value)](#setByRateType-int-com.aspose.tasks.RateByDateCollection-) | Establece el elemento en el índice especificado. |
| [size()](#size--) | Obtiene el número de elementos contenidos en la RateCollection. |
| [toList()](#toList--) | Convierte el objeto [RateCollection](../../com.aspose.tasks/ratecollection) en una lista de objetos [Rate](../../com.aspose.tasks/rate). |
| [toList(int type)](#toList-int-) | Convierte el objeto [RateCollection](../../com.aspose.tasks/ratecollection) en una lista de objetos [Rate](../../com.aspose.tasks/rate) filtrados por el tipo [RateType](../../com.aspose.tasks/ratetype) especificado. |
### add(Date ratesFrom) {#add-java.util.Date-}
```
public final Rate add(Date ratesFrom)
```


Agrega una nueva instancia de [Rate](../../com.aspose.tasks/rate) a esta colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ratesFrom | java.util.Date | La fecha en que la nueva tarifa entra en vigor. |

**Returns:**
[Rate](../../com.aspose.tasks/rate) - Added [Rate](../../com.aspose.tasks/rate) instance.
### add(Date ratesFrom, int type) {#add-java.util.Date-int-}
```
public final Rate add(Date ratesFrom, int type)
```


Agrega una nueva instancia de [Rate](../../com.aspose.tasks/rate) a esta colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ratesFrom | java.util.Date | La fecha en que la nueva tarifa entra en vigor. |
| type | int | La tabla de tarifas a la que se añadirá. |

**Returns:**
[Rate](../../com.aspose.tasks/rate) - Added [Rate](../../com.aspose.tasks/rate) instance.
### clear() {#clear--}
```
public final void clear()
```




### entrySet() {#entrySet--}
```
public Set<Map.Entry<Integer,RateByDateCollection>> entrySet()
```


(@inheritDoc\}

**Returns:**
java.util.Set&lt;java.util.Map.Entry&lt;java.lang.Integer,com.aspose.tasks.RateByDateCollection&gt;&gt; - \{@inheritDoc\}
### get(Object key) {#get-java.lang.Object-}
```
public final RateByDateCollection get(Object key)
```


(@inheritDoc\}

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| key | java.lang.Object | \{@inheritDoc\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### getByRateType(int key) {#getByRateType-int-}
```
public final RateByDateCollection getByRateType(int key)
```


Devuelve el elemento en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| key | int | El índice basado en cero del elemento a obtener. |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - the element at the specified index.
### getParentResource() {#getParentResource--}
```
public final Resource getParentResource()
```


Obtiene el objeto [Resource](../../com.aspose.tasks/resource) padre para esta colección.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - the parent [Resource](../../com.aspose.tasks/resource) object for this collection.
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Obtiene un valor que indica si esta colección es de solo lectura.

**Returns:**
boolean - un valor que indica si esta colección es de solo lectura.
### iterator() {#iterator--}
```
public final Iterator iterator()
```


Devuelve un enumerador para esta colección.

**Returns:**
java.util.Iterator - un enumerador para esta colección.
### put(Integer key, RateByDateCollection value) {#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-}
```
public final RateByDateCollection put(Integer key, RateByDateCollection value)
```


(@inheritDoc\}

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| key | java.lang.Integer | \{@inheritDoc\} |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | \{@inheritDoc\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### remove(Rate item) {#remove-com.aspose.tasks.Rate-}
```
public final boolean remove(Rate item)
```


Elimina la instancia de Rate de esta colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| item | [Rate](../../com.aspose.tasks/rate) | El elemento a eliminar. |

**Returns:**
boolean - true si la Rate especificada se eliminó correctamente; de lo contrario, false.
### setByRateType(int key, RateByDateCollection value) {#setByRateType-int-com.aspose.tasks.RateByDateCollection-}
```
public final void setByRateType(int key, RateByDateCollection value)
```


Establece el elemento en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| key | int | El índice basado en cero del elemento a establecer. |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | El elemento a establecer en el índice especificado. |

### size() {#size--}
```
public final int size()
```


Obtiene el número de elementos contenidos en la RateCollection.

**Returns:**
int - el número de elementos contenidos en RateCollection.
### toList() {#toList--}
```
public final List<Rate> toList()
```


Convierte el objeto [RateCollection](../../com.aspose.tasks/ratecollection) en una lista de objetos [Rate](../../com.aspose.tasks/rate).

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - Lista de objetos [Rate](../../com.aspose.tasks/rate).
### toList(int type) {#toList-int-}
```
public final List<Rate> toList(int type)
```


Convierte el objeto [RateCollection](../../com.aspose.tasks/ratecollection) en una lista de objetos [Rate](../../com.aspose.tasks/rate) filtrados por el tipo [RateType](../../com.aspose.tasks/ratetype) especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | int | El tipo por el cual filtrar. |

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - una lista de objetos [Rate](../../com.aspose.tasks/rate).
