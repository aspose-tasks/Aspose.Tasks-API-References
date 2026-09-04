---
title: "ArrayUtils"
second_title: "Aspose.Tasks for Java API Reference"
description: "Hilfsklasse für die Verarbeitung von ArrayList."
type: docs
weight: 14
url: /de/java/com.aspose.tasks/arrayutils/
---

**Inheritance:**
java.lang.Object
```
public class ArrayUtils
```

Hilfsklasse für die Verarbeitung von ArrayList.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [&lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[][] arrays)](#-T-concat-java.lang.Class-T--T--...-) |  |
| [apply(List array, IAlgorithm algorithm, int startIndex)](#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-) | Algorithmus für jedes Listenelement ab der angegebenen Position anwenden. |
| [filter(List array, ICondition cond)](#filter-java.util.List-com.aspose.tasks.ICondition-) | ArrayList-Elemente nach der angegebenen Bedingung filtern. |
| [find(List array, ICondition cond)](#find-java.util.List-com.aspose.tasks.ICondition-) | Finde das erste Vorkommen eines ArrayList-Elements, das die angegebene Bedingung erfüllt. |
### &lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[][] arrays) {#-T-concat-java.lang.Class-T--T--...-}
```
public static T[] <T>concat(Class<T> typeOfT, T[][] arrays)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| typeOfT | java.lang.Class&lt;T&gt; |  |
| Arrays | T[][] |  |

**Returns:**
T[]
### apply(List array, IAlgorithm algorithm, int startIndex) {#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-}
```
public static void apply(List array, IAlgorithm algorithm, int startIndex)
```


Algorithmus für jedes Listenelement ab der angegebenen Position anwenden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Array | java.util.List | ArrayList zu verarbeiten. |
| Algorithmus | com.aspose.tasks.IAlgorithm | Angewendeter Algorithmus. |
| startIndex | int | Startposition des Elements. |

### filter(List array, ICondition cond) {#filter-java.util.List-com.aspose.tasks.ICondition-}
```
public static List filter(List array, ICondition cond)
```


ArrayList-Elemente nach der angegebenen Bedingung filtern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Array | java.util.List | Liste zur Verarbeitung. |
| cond | com.aspose.tasks.ICondition | Bedingung zum Filtern der List. |

**Returns:**
java.util.List - Gefilterte Liste.
### find(List array, ICondition cond) {#find-java.util.List-com.aspose.tasks.ICondition-}
```
public static Object find(List array, ICondition cond)
```


Finde das erste Vorkommen eines ArrayList-Elements, das die angegebene Bedingung erfüllt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Array | java.util.List | ArrayList zu verarbeiten. |
| cond | com.aspose.tasks.ICondition | Bedingung zum Finden des ArrayList-Elements. |

**Returns:**
java.lang.Object - List-Element oder null.
