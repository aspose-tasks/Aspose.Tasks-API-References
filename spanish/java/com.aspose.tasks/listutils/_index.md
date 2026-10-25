---
title: "ListUtils"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Clase de utilidad para el procesamiento de listas."
type: docs
weight: 147
url: /es/java/com.aspose.tasks/listutils/
---

**Inheritance:**
java.lang.Object
```
public class ListUtils
```

Clase de utilidad para el procesamiento de listas.
## Métodos

| Método | Descripción |
| --- | --- |
| [&lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex)](#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-) | Aplica el algoritmo a cada elemento de la lista a partir de la posición especificada. |
| [&lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond)](#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--) | Filtra los elementos de la lista según la condición especificada. |
| [&lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz)](#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-) | Encuentra la primera ocurrencia de un elemento de la lista que cumpla la condición especificada. |
### &lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex) {#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-}
```
public static void <T>apply(List<T> list, IAlgorithm<T> algorithm, int startIndex)
```


Aplica el algoritmo a cada elemento de la lista a partir de la posición especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| lista | java.util.List&lt;T&gt; | Lista a procesar. |
| algorithm | [IAlgorithm](../../com.aspose.tasks/ialgorithm) | Algoritmo aplicado. |
| startIndex | int | Posición del elemento inicial. |

### &lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond) {#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--}
```
public static List<T> <T>filter(List<T> list, ICondition<T> cond)
```


Filtra los elementos de la lista según la condición especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| lista | java.util.List&lt;T&gt; | Una lista a procesar. |
| cond | [ICondition](../../com.aspose.tasks/icondition) | Condición utilizada para filtrar la lista especificada. |

**Returns:**
java.util.List&lt;T&gt; - Lista filtrada.
### &lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz) {#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-}
```
public static T <T>find(List<T> list, ICondition<T> cond, Class clazz)
```


Encuentra la primera ocurrencia de un elemento de la lista que cumpla la condición especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| lista | java.util.List&lt;T&gt; | Una lista a procesar. |
| cond | [ICondition](../../com.aspose.tasks/icondition) | Condición utilizada para encontrar un elemento en la lista especificada. |
| clazz | java.lang.Class | Tipo de clase del elemento T. |

**Returns:**
T - elemento de lista o nulo.
