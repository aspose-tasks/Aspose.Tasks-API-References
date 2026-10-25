---
title: "RiskItemStatisticsCollection"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa una colección que contiene las instancias de la clase."
type: docs
weight: 266
url: /es/java/com.aspose.tasks/riskitemstatisticscollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.util.Map, java.lang.Iterable
```
public class RiskItemStatisticsCollection implements Map<Task,RiskItemStatistics>, Iterable<RiskItemStatistics>
```

Representa una colección que contiene las instancias de la clase [RiskItemStatistics](../../com.aspose/tasks/riskitemstatistics).
## Métodos

| Método | Descripción |
| --- | --- |
| [clear()](#clear--) | Elimina todos los elementos de la colección. |
| [containsKey(Object key)](#containsKey-java.lang.Object-) | Devuelve true si este mapa contiene una asignación para la clave especificada. |
| [containsValue(Object value)](#containsValue-java.lang.Object-) | Devuelve true si este mapa asigna una o más claves al valor especificado. |
| [entrySet()](#entrySet--) | Devuelve una vista Set de las asignaciones contenidas en este mapa. |
| [get(Object task)](#get-java.lang.Object-) | Devuelve una instancia de la clase `RiskItemStatistics` contenida en esta colección que está asociada con el objeto Task especificado; null si no se encuentra el elemento. |
| [isEmpty()](#isEmpty--) | Devuelve true si este mapa no contiene asignaciones clave-valor |
| [iterator()](#iterator--) | Devuelve un enumerador para esta colección. |
| [keySet()](#keySet--) | Devuelve una vista Set de las claves contenidas en este mapa. |
| [put(Task key, RiskItemStatistics value)](#put-com.aspose.tasks.Task-com.aspose.tasks.RiskItemStatistics-) | Asocia el valor especificado con la clave especificada en este mapa. |
| [putAll(Map&lt;? extends Task,? extends RiskItemStatistics&gt; m)](#putAll-java.util.Map---extends-com.aspose.tasks.Task---extends-com.aspose.tasks.RiskItemStatistics--) | Copia todas las asignaciones del mapa especificado a este mapa. |
| [remove(Object key)](#remove-java.lang.Object-) | Elimina la asignación de una clave de este mapa si está presente. |
| [size()](#size--) | Devuelve el número de elementos en esta colección. |
| [values()](#values--) | Devuelve una vista Collection de los valores contenidos en este mapa. |
### clear() {#clear--}
```
public void clear()
```


Elimina todos los elementos de la colección.

### containsKey(Object key) {#containsKey-java.lang.Object-}
```
public boolean containsKey(Object key)
```


Devuelve true si este mapa contiene una asignación para la clave especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| key | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - true si este mapa contiene una asignación para la clave especificada.
### containsValue(Object value) {#containsValue-java.lang.Object-}
```
public boolean containsValue(Object value)
```


Devuelve true si este mapa asigna una o más claves al valor especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - true si este mapa asigna una o más claves al valor especificado.
### entrySet() {#entrySet--}
```
public Set<Map.Entry<Task,RiskItemStatistics>> entrySet()
```


Devuelve una vista Set de las asignaciones contenidas en este mapa.

**Returns:**
java.util.Set&lt;java.util.Map.Entry&lt;com.aspose.tasks.Task,com.aspose.tasks.RiskItemStatistics&gt;&gt; - \{@inheritDoc\}
### get(Object task) {#get-java.lang.Object-}
```
public RiskItemStatistics get(Object task)
```


Devuelve una instancia de la clase `RiskItemStatistics` contenida en esta colección que está asociada con el objeto Task especificado; null si no se encuentra el elemento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tarea | java.lang.Object | la instancia especificada de la clase `Task`. |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - risk item which is associated with the specified task object if found; null otherwise.
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Devuelve true si este mapa no contiene asignaciones clave-valor

**Returns:**
boolean - verdadero si este mapa no contiene asignaciones clave-valor
### iterator() {#iterator--}
```
public Iterator<RiskItemStatistics> iterator()
```


Devuelve un enumerador para esta colección.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.RiskItemStatistics&gt; - un enumerador para esta colección.
### keySet() {#keySet--}
```
public Set<Task> keySet()
```


Devuelve una vista Set de las claves contenidas en este mapa.

**Returns:**
java.util.Set&lt;com.aspose.tasks.Task&gt; - una vista de conjunto de las claves contenidas en este mapa.
### put(Task key, RiskItemStatistics value) {#put-com.aspose.tasks.Task-com.aspose.tasks.RiskItemStatistics-}
```
public RiskItemStatistics put(Task key, RiskItemStatistics value)
```


Asocia el valor especificado con la clave especificada en este mapa.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| key | [Task](../../com.aspose.tasks/task) | \{@inheritDoc\} |
| value | [RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) | \{@inheritDoc\} |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - \{@inheritDoc\}
### putAll(Map&lt;? extends Task,? extends RiskItemStatistics&gt; m) {#putAll-java.util.Map---extends-com.aspose.tasks.Task---extends-com.aspose.tasks.RiskItemStatistics--}
```
public void putAll(Map<? extends Task,? extends RiskItemStatistics> m)
```


Copia todas las asignaciones del mapa especificado a este mapa.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| m | java.util.Map&lt;? extends com.aspose.tasks.Task,? extends com.aspose.tasks.RiskItemStatistics&gt; | \{@inheritDoc\} |

### remove(Object key) {#remove-java.lang.Object-}
```
public RiskItemStatistics remove(Object key)
```


Elimina la asignación de una clave de este mapa si está presente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| key | java.lang.Object | \{@inheritDoc\} |

**Returns:**
[RiskItemStatistics](../../com.aspose.tasks/riskitemstatistics) - \{@inheritDoc\}
### size() {#size--}
```
public int size()
```


Devuelve el número de elementos en esta colección.

**Returns:**
int - el número de elementos en esta colección.
### values() {#values--}
```
public Collection<RiskItemStatistics> values()
```


Devuelve una vista Collection de los valores contenidos en este mapa.

**Returns:**
java.util.Collection&lt;com.aspose.tasks.RiskItemStatistics&gt; - una vista de colección de los valores contenidos en este mapa.
