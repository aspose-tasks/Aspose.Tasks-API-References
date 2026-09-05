---
title: "ListUtils"
second_title: "Aspose.Tasks for Java API Reference"
description: "Classe di utilità per l'elaborazione delle liste."
type: docs
weight: 147
url: /it/java/com.aspose.tasks/listutils/
---

**Inheritance:**
java.lang.Object
```
public class ListUtils
```

Classe di utilità per l'elaborazione delle liste.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [&lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex)](#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-) | Applica l'algoritmo a ciascun elemento della lista a partire dalla posizione specificata. |
| [&lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond)](#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--) | Filtra gli elementi della lista in base alla condizione specificata. |
| [&lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz)](#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-) | Trova la prima occorrenza di un elemento della lista che soddisfa la condizione specificata. |
### &lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex) {#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-}
```
public static void <T>apply(List<T> list, IAlgorithm<T> algorithm, int startIndex)
```


Applica l'algoritmo a ciascun elemento della lista a partire dalla posizione specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| elenco | java.util.List&lt;T&gt; | Elenco da elaborare. |
| algorithm | [IAlgorithm](../../com.aspose.tasks/ialgorithm) | Algoritmo applicato. |
| indiceInizio | int | Posizione dell'elemento iniziale. |

### &lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond) {#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--}
```
public static List<T> <T>filter(List<T> list, ICondition<T> cond)
```


Filtra gli elementi della lista in base alla condizione specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| elenco | java.util.List&lt;T&gt; | Una lista da elaborare. |
| cond | [ICondition](../../com.aspose.tasks/icondition) | Condizione usata per filtrare la lista specificata. |

**Returns:**
java.util.List&lt;T&gt; - Lista filtrata.
### &lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz) {#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-}
```
public static T <T>find(List<T> list, ICondition<T> cond, Class clazz)
```


Trova la prima occorrenza di un elemento della lista che soddisfa la condizione specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| elenco | java.util.List&lt;T&gt; | Una lista da elaborare. |
| cond | [ICondition](../../com.aspose.tasks/icondition) | Condizione usata per trovare un elemento nella lista specificata. |
| clazz | java.lang.Class | Tipo di classe dell'elemento T. |

**Returns:**
T - elemento della lista o null.
