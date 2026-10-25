---
title: "ListUtils"
second_title: "Aspose.Tasks for Java API-referens"
description: "Verktygsklass för listbehandling."
type: docs
weight: 147
url: /sv/java/com.aspose.tasks/listutils/
---

**Inheritance:**
java.lang.Object
```
public class ListUtils
```

Verktygsklass för listbehandling.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [&lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex)](#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-) | Applicera algoritm för varje listelement med start från angiven position. |
| [&lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond)](#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--) | Filtrera listelement efter angivet villkor. |
| [&lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz)](#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-) | Hitta första förekomsten av ett listelement som uppfyller angivet villkor. |
### &lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex) {#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-}
```
public static void <T>apply(List<T> list, IAlgorithm<T> algorithm, int startIndex)
```


Applicera algoritm för varje listelement med start från angiven position.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| lista | java.util.List&lt;T&gt; | Lista att bearbeta. |
| algorithm | [IAlgorithm](../../com.aspose.tasks/ialgorithm) | Tillämpad algoritm. |
| startIndex | int | Startposition för elementet. |

### &lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond) {#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--}
```
public static List<T> <T>filter(List<T> list, ICondition<T> cond)
```


Filtrera listelement efter angivet villkor.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| lista | java.util.List&lt;T&gt; | En lista att bearbeta. |
| cond | [ICondition](../../com.aspose.tasks/icondition) | Villkor som används för att filtrera den angivna listan. |

**Returns:**
java.util.List&lt;T&gt; - Filtrerad lista.
### &lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz) {#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-}
```
public static T <T>find(List<T> list, ICondition<T> cond, Class clazz)
```


Hitta första förekomsten av ett listelement som uppfyller angivet villkor.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| lista | java.util.List&lt;T&gt; | En lista att bearbeta. |
| cond | [ICondition](../../com.aspose.tasks/icondition) | Villkor som används för att hitta ett element i den angivna listan. |
| clazz | java.lang.Class | Klasstyp för elementet T. |

**Returns:**
T - Listelement eller null.
