---
title: "ArrayUtils"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Clase de utilidad para el procesamiento de ArrayList."
type: docs
weight: 14
url: /es/java/com.aspose.tasks/arrayutils/
---

**Inheritance:**
java.lang.Object
```
public class ArrayUtils
```

Clase de utilidad para el procesamiento de ArrayList.
## Métodos

| Método | Descripción |
| --- | --- |
| [&lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[][] arrays)](#-T-concat-java.lang.Class-T--T--...-) |  |
| [apply(List array, IAlgorithm algorithm, int startIndex)](#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-) | Aplicar algoritmo para cada elemento de la lista a partir de la posición especificada. |
| [filter(List array, ICondition cond)](#filter-java.util.List-com.aspose.tasks.ICondition-) | Filtrar elementos de ArrayList según la condición especificada. |
| [find(List array, ICondition cond)](#find-java.util.List-com.aspose.tasks.ICondition-) | Encontrar la primera aparición de un elemento de ArrayList que cumpla la condición especificada. |
### &lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[][] arrays) {#-T-concat-java.lang.Class-T--T--...-}
```
public static T[] <T>concat(Class<T> typeOfT, T[][] arrays)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| typeOfT | java.lang.Class&lt;T&gt; |  |
| arreglos | T[][] |  |

**Returns:**
T[]
### apply(List array, IAlgorithm algorithm, int startIndex) {#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-}
```
public static void apply(List array, IAlgorithm algorithm, int startIndex)
```


Aplicar algoritmo para cada elemento de la lista a partir de la posición especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| array | java.util.List | ArrayList a procesar. |
| algoritmo | com.aspose.tasks.IAlgorithm | Algoritmo aplicado. |
| startIndex | int | Posición del elemento inicial. |

### filter(List array, ICondition cond) {#filter-java.util.List-com.aspose.tasks.ICondition-}
```
public static List filter(List array, ICondition cond)
```


Filtrar elementos de ArrayList según la condición especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| array | java.util.List | Lista a procesar. |
| cond | com.aspose.tasks.ICondition | Condición usada para filtrar la lista. |

**Returns:**
java.util.List - Lista filtrada.
### find(List array, ICondition cond) {#find-java.util.List-com.aspose.tasks.ICondition-}
```
public static Object find(List array, ICondition cond)
```


Encontrar la primera aparición de un elemento de ArrayList que cumpla la condición especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| array | java.util.List | ArrayList a procesar. |
| cond | com.aspose.tasks.ICondition | Condición usada para encontrar un elemento de ArrayList. |

**Returns:**
java.lang.Object - Elemento de lista o nulo.
