---
title: "TimephasedDataCollection"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa una colección de objetos."
type: docs
weight: 321
url: /es/java/com.aspose.tasks/timephaseddatacollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public abstract class TimephasedDataCollection extends AbstractList<TimephasedData>
```

Representa una colección de objetos [TimephasedData](../../com.aspose.tasks/timephaseddata).
## Constructores

| Constructor | Descripción |
| --- | --- |
| [TimephasedDataCollection()](#TimephasedDataCollection--) | Inicializa una nueva instancia de la clase [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection). |
## Métodos

| Método | Descripción |
| --- | --- |
| [add(TimephasedData item)](#add-com.aspose.tasks.TimephasedData-) | Agrega una instancia de [TimephasedData](../../com.aspose.tasks/timephaseddata) a este objeto de colección. |
| [addRange(Iterable&lt;TimephasedData&gt; timephasedCollection)](#addRange-java.lang.Iterable-com.aspose.tasks.TimephasedData--) | Agrega una colección de instancias de [TimephasedData](../../com.aspose.tasks/timephaseddata) a este objeto de colección. |
| [clear()](#clear--) | Elimina todos los elementos de la [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection). |
| [containsItem(TimephasedData item)](#containsItem-com.aspose.tasks.TimephasedData-) | Determina si la [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) contiene un valor específico. |
| [copyToTArray(TimephasedData[] array, int arrayIndex)](#copyToTArray-com.aspose.tasks.TimephasedData---int-) | Copia los elementos de la [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) a una Array, comenzando en un índice de Array particular. |
| [get(int index)](#get-int-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Obtiene un valor que indica si el System.Collections.Generic.ICollection&lt;T&gt; es de solo lectura. |
| [iterator()](#iterator--) | Devuelve un iterador para esta colección. |
| [remove(TimephasedData item)](#remove-com.aspose.tasks.TimephasedData-) | Elimina la instancia de [TimephasedData](../../com.aspose.tasks/timephaseddata) de este objeto de colección. |
| [selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime)](#selectBetweenStartAndFinish-byte-java.util.Date-java.util.Date-) | Selecciona todas las fases de tiempo entre `startTime` y `finishTime`. |
| [set_Item(int index, TimephasedData value)](#set-Item-int-com.aspose.tasks.TimephasedData-) | Establece el elemento en el índice especificado. |
| [size()](#size--) | Obtiene el número de objetos contenidos en este objeto [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection). |
| [toList()](#toList--) | Convierte el objeto [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) a una lista de objetos [TimephasedData](../../com.aspose.tasks/timephaseddata). |
### TimephasedDataCollection() {#TimephasedDataCollection--}
```
public TimephasedDataCollection()
```


Inicializa una nueva instancia de la clase [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection).

### add(TimephasedData item) {#add-com.aspose.tasks.TimephasedData-}
```
public final boolean add(TimephasedData item)
```


Agrega una instancia de [TimephasedData](../../com.aspose.tasks/timephaseddata) a este objeto de colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | El elemento a añadir. |

**Returns:**
boolean - true, si el elemento fue agregado; de lo contrario, false.
### addRange(Iterable&lt;TimephasedData&gt; timephasedCollection) {#addRange-java.lang.Iterable-com.aspose.tasks.TimephasedData--}
```
public final void addRange(Iterable<TimephasedData> timephasedCollection)
```


Agrega una colección de instancias de [TimephasedData](../../com.aspose.tasks/timephaseddata) a este objeto de colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| timephasedCollection | java.lang.Iterable&lt;com.aspose.tasks.TimephasedData&gt; | Una colección de objetos [TimephasedData](../../com.aspose.tasks/timephaseddata) para agregar. |

### clear() {#clear--}
```
public final void clear()
```


Elimina todos los elementos de la [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection).

### containsItem(TimephasedData item) {#containsItem-com.aspose.tasks.TimephasedData-}
```
public final boolean containsItem(TimephasedData item)
```


Determina si la [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) contiene un valor específico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | El objeto a localizar en la colección. |

**Returns:**
boolean - true si `item` se encuentra en la colección; de lo contrario, false.
### copyToTArray(TimephasedData[] array, int arrayIndex) {#copyToTArray-com.aspose.tasks.TimephasedData---int-}
```
public final void copyToTArray(TimephasedData[] array, int arrayIndex)
```


Copia los elementos de la [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) a una Array, comenzando en un índice de Array particular.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| array | [TimephasedData\[\]](../../com.aspose.tasks/timephaseddata) | La matriz unidimensional que es el destino de los elementos copiados de [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection). La matriz debe tener indexación basada en cero. |
| arrayIndex | int | El índice basado en cero en `array` en el que comienza la copia. |

### get(int index) {#get-int-}
```
public TimephasedData get(int index)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | \{@inheritDoc\} |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Obtiene un valor que indica si el System.Collections.Generic.ICollection&lt;T&gt; es de solo lectura.

**Returns:**
boolean - verdadero si la System.Collections.Generic.ICollection&lt;T&gt; es de solo lectura; de lo contrario, falso.
### iterator() {#iterator--}
```
public final Iterator<TimephasedData> iterator()
```


Devuelve un iterador para esta colección.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.TimephasedData&gt; - un iterador para esta colección.
### remove(TimephasedData item) {#remove-com.aspose.tasks.TimephasedData-}
```
public final boolean remove(TimephasedData item)
```


Elimina la instancia de [TimephasedData](../../com.aspose.tasks/timephaseddata) de este objeto de colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | El elemento a eliminar. |

**Returns:**
boolean - verdadero si `item` se eliminó correctamente de la [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection); de lo contrario, falso. Este método también devuelve falso si `item` no se encuentra en la [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection).
### selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime) {#selectBetweenStartAndFinish-byte-java.util.Date-java.util.Date-}
```
public final List<TimephasedData> selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime)
```


Selecciona todas las fases de tiempo entre `startTime` y `finishTime`. Tiene complejidad O(log n) en el caso promedio.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| timephasedDataType | byte | Tipo de fases de tiempo a seleccionar. |
| startTime | java.util.Date | Inicio del intervalo. |
| finishTime | java.util.Date | Fin del intervalo. |

**Returns:**
java.util.List&lt;com.aspose.tasks.TimephasedData&gt; - Devuelve una nueva instancia de lista de los datos de [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) ordenados por la propiedad Start.
### set_Item(int index, TimephasedData value) {#set-Item-int-com.aspose.tasks.TimephasedData-}
```
public final void set_Item(int index, TimephasedData value)
```


Establece el elemento en el índice especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice basado en cero del elemento a establecer. |
| value | [TimephasedData](../../com.aspose.tasks/timephaseddata) | el elemento a establecer. |

### size() {#size--}
```
public final int size()
```


Obtiene el número de objetos contenidos en este objeto [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection).

**Returns:**
int - el número de objetos contenidos en este objeto [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection).
### toList() {#toList--}
```
public final List<TimephasedData> toList()
```


Convierte el objeto [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) a una lista de objetos [TimephasedData](../../com.aspose.tasks/timephaseddata).

**Returns:**
java.util.List&lt;com.aspose.tasks.TimephasedData&gt; - Lista de objetos [TimephasedData](../../com.aspose.tasks/timephaseddata).
