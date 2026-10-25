---
title: "ListUtils"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Hulpprogrammaklasse voor lijstverwerking."
type: docs
weight: 147
url: /nl/java/com.aspose.tasks/listutils/
---

**Inheritance:**
java.lang.Object
```
public class ListUtils
```

Hulpprogrammaklasse voor lijstverwerking.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [&lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex)](#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-) | Pas algoritme toe op elk lijst‑element beginnend vanaf de opgegeven positie. |
| [&lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond)](#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--) | Filter lijst‑elementen op basis van de opgegeven voorwaarde. |
| [&lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz)](#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-) | Vind de eerste voorkoming van een lijst‑element dat aan de opgegeven voorwaarde voldoet. |
### &lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex) {#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-}
```
public static void <T>apply(List<T> list, IAlgorithm<T> algorithm, int startIndex)
```


Pas algoritme toe op elk lijst‑element beginnend vanaf de opgegeven positie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| lijst | java.util.List&lt;T&gt; | Lijst om te verwerken. |
| algorithm | [IAlgorithm](../../com.aspose.tasks/ialgorithm) | Toegepast algoritme. |
| startIndex | int | Startpositie van het element. |

### &lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond) {#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--}
```
public static List<T> <T>filter(List<T> list, ICondition<T> cond)
```


Filter lijst‑elementen op basis van de opgegeven voorwaarde.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| lijst | java.util.List&lt;T&gt; | Een lijst om te verwerken. |
| cond | [ICondition](../../com.aspose.tasks/icondition) | Voorwaarde die wordt gebruikt om de opgegeven lijst te filteren. |

**Returns:**
java.util.List&lt;T&gt; - Gefilterde lijst.
### &lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz) {#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-}
```
public static T <T>find(List<T> list, ICondition<T> cond, Class clazz)
```


Vind de eerste voorkoming van een lijst‑element dat aan de opgegeven voorwaarde voldoet.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| lijst | java.util.List&lt;T&gt; | Een lijst om te verwerken. |
| cond | [ICondition](../../com.aspose.tasks/icondition) | Voorwaarde die wordt gebruikt om een element in de opgegeven lijst te vinden. |
| clazz | java.lang.Class | Klasse‑type van element T. |

**Returns:**
T - Lijstonderdeel of null.
