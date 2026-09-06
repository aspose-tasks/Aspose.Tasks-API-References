---
title: "ArrayUtils"
second_title: "Aspose.Tasks for Java API-referens"
description: "Verktygsklass för bearbetning av ArrayList."
type: docs
weight: 14
url: /sv/java/com.aspose.tasks/arrayutils/
---

**Inheritance:**
java.lang.Object
```
public class ArrayUtils
```

Verktygsklass för bearbetning av ArrayList.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [&lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[][] arrays)](#-T-concat-java.lang.Class-T--T--...-) |  |
| [apply(List array, IAlgorithm algorithm, int startIndex)](#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-) | Applicera algoritm för varje List-element med början från angiven position. |
| [filter(List array, ICondition cond)](#filter-java.util.List-com.aspose.tasks.ICondition-) | Filtrera ArrayList-element efter angivet villkor. |
| [find(List array, ICondition cond)](#find-java.util.List-com.aspose.tasks.ICondition-) | Hitta första förekomsten av ett ArrayList-element som uppfyller det angivna villkoret. |
### &lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[][] arrays) {#-T-concat-java.lang.Class-T--T--...-}
```
public static T[] <T>concat(Class<T> typeOfT, T[][] arrays)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typeOfT | java.lang.Class&lt;T&gt; |  |
| arrayer | T[][] |  |

**Returns:**
T[]
### apply(List array, IAlgorithm algorithm, int startIndex) {#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-}
```
public static void apply(List array, IAlgorithm algorithm, int startIndex)
```


Applicera algoritm för varje List-element med början från angiven position.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| array | java.util.List | ArrayList att bearbeta. |
| algoritm | com.aspose.tasks.IAlgorithm | Tillämpad algoritm. |
| startIndex | int | Startposition för elementet. |

### filter(List array, ICondition cond) {#filter-java.util.List-com.aspose.tasks.ICondition-}
```
public static List filter(List array, ICondition cond)
```


Filtrera ArrayList-element efter angivet villkor.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| array | java.util.List | Lista att bearbeta. |
| cond | com.aspose.tasks.ICondition | Villkor som används för att filtrera List. |

**Returns:**
java.util.List - Filtrerad List.
### find(List array, ICondition cond) {#find-java.util.List-com.aspose.tasks.ICondition-}
```
public static Object find(List array, ICondition cond)
```


Hitta första förekomsten av ett ArrayList-element som uppfyller det angivna villkoret.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| array | java.util.List | ArrayList att bearbeta. |
| cond | com.aspose.tasks.ICondition | Villkor som används för att hitta ArrayList-element. |

**Returns:**
java.lang.Object - List-element eller null.
