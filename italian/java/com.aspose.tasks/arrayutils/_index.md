---
title: "ArrayUtils"
second_title: "Aspose.Tasks for Java API Reference"
description: "Classe di utilità per l'elaborazione di ArrayList."
type: docs
weight: 14
url: /it/java/com.aspose.tasks/arrayutils/
---

**Inheritance:**
java.lang.Object
```
public class ArrayUtils
```

Classe di utilità per l'elaborazione di ArrayList.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [&lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[][] arrays)](#-T-concat-java.lang.Class-T--T--...-) |  |
| [apply(List array, IAlgorithm algorithm, int startIndex)](#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-) | Applica l'algoritmo a ciascun elemento della lista a partire dalla posizione specificata. |
| [filter(List array, ICondition cond)](#filter-java.util.List-com.aspose.tasks.ICondition-) | Filtra gli elementi di ArrayList secondo la condizione specificata. |
| [find(List array, ICondition cond)](#find-java.util.List-com.aspose.tasks.ICondition-) | Trova la prima occorrenza di un elemento di ArrayList che soddisfa la condizione specificata. |
### &lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[][] arrays) {#-T-concat-java.lang.Class-T--T--...-}
```
public static T[] <T>concat(Class<T> typeOfT, T[][] arrays)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| typeOfT | java.lang.Class&lt;T&gt; |  |
| array | T[][] |  |

**Returns:**
T[]
### apply(List array, IAlgorithm algorithm, int startIndex) {#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-}
```
public static void apply(List array, IAlgorithm algorithm, int startIndex)
```


Applica l'algoritmo a ciascun elemento della lista a partire dalla posizione specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| array | java.util.List | ArrayList da elaborare. |
| algoritmo | com.aspose.tasks.IAlgorithm | Algoritmo applicato. |
| indiceInizio | int | Posizione dell'elemento iniziale. |

### filter(List array, ICondition cond) {#filter-java.util.List-com.aspose.tasks.ICondition-}
```
public static List filter(List array, ICondition cond)
```


Filtra gli elementi di ArrayList secondo la condizione specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| array | java.util.List | Elenco da elaborare. |
| cond | com.aspose.tasks.ICondition | Condizione usata per filtrare la lista. |

**Returns:**
java.util.List - Lista filtrata.
### find(List array, ICondition cond) {#find-java.util.List-com.aspose.tasks.ICondition-}
```
public static Object find(List array, ICondition cond)
```


Trova la prima occorrenza di un elemento di ArrayList che soddisfa la condizione specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| array | java.util.List | ArrayList da elaborare. |
| cond | com.aspose.tasks.ICondition | Condizione usata per trovare l'elemento di ArrayList. |

**Returns:**
java.lang.Object - Elemento della lista o null.
