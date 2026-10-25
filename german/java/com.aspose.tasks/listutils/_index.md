---
title: "ListUtils"
second_title: "Aspose.Tasks for Java API Reference"
description: "Hilfsklasse für die Listenverarbeitung."
type: docs
weight: 147
url: /de/java/com.aspose.tasks/listutils/
---

**Inheritance:**
java.lang.Object
```
public class ListUtils
```

Hilfsklasse für die Listenverarbeitung.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [&lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex)](#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-) | Algorithmus für jedes Listenelement ab der angegebenen Position anwenden. |
| [&lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond)](#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--) | Listenelemente nach der angegebenen Bedingung filtern. |
| [&lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz)](#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-) | Erstes Vorkommen eines Listenelements finden, das die angegebene Bedingung erfüllt. |
### &lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex) {#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-}
```
public static void <T>apply(List<T> list, IAlgorithm<T> algorithm, int startIndex)
```


Algorithmus für jedes Listenelement ab der angegebenen Position anwenden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Liste | java.util.List&lt;T&gt; | Liste zur Verarbeitung. |
| algorithm | [IAlgorithm](../../com.aspose.tasks/ialgorithm) | Angewendeter Algorithmus. |
| startIndex | int | Startposition des Elements. |

### &lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond) {#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--}
```
public static List<T> <T>filter(List<T> list, ICondition<T> cond)
```


Listenelemente nach der angegebenen Bedingung filtern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Liste | java.util.List&lt;T&gt; | Eine Liste zur Verarbeitung. |
| cond | [ICondition](../../com.aspose.tasks/icondition) | Bedingung, die zum Filtern der angegebenen Liste verwendet wird. |

**Returns:**
java.util.List&lt;T&gt; - Gefilterte Liste.
### &lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz) {#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-}
```
public static T <T>find(List<T> list, ICondition<T> cond, Class clazz)
```


Erstes Vorkommen eines Listenelements finden, das die angegebene Bedingung erfüllt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Liste | java.util.List&lt;T&gt; | Eine Liste zur Verarbeitung. |
| cond | [ICondition](../../com.aspose.tasks/icondition) | Bedingung, die zum Finden eines Elements in der angegebenen Liste verwendet wird. |
| clazz | java.lang.Class | Klassentyp des Elements T. |

**Returns:**
T - Listenelement oder null.
