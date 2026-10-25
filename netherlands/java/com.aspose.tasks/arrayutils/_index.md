---
title: "ArrayUtils"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Hulpprogrammaklasse voor ArrayList-verwerking."
type: docs
weight: 14
url: /nl/java/com.aspose.tasks/arrayutils/
---

**Inheritance:**
java.lang.Object
```
public class ArrayUtils
```

Hulpprogrammaklasse voor ArrayList-verwerking.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [&lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[][] arrays)](#-T-concat-java.lang.Class-T--T--...-) |  |
| [apply(List array, IAlgorithm algorithm, int startIndex)](#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-) | Pas algoritme toe op elk lijstonderdeel beginnend vanaf de opgegeven positie. |
| [filter(List array, ICondition cond)](#filter-java.util.List-com.aspose.tasks.ICondition-) | Filter ArrayList-elementen op basis van de opgegeven voorwaarde. |
| [find(List array, ICondition cond)](#find-java.util.List-com.aspose.tasks.ICondition-) | Vind de eerste voorkoming van een ArrayList-element dat voldoet aan de opgegeven voorwaarde. |
### &lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[][] arrays) {#-T-concat-java.lang.Class-T--T--...-}
```
public static T[] <T>concat(Class<T> typeOfT, T[][] arrays)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| typeOfT | java.lang.Class&lt;T&gt; |  |
| arrays | T[][] |  |

**Returns:**
T[]
### apply(List array, IAlgorithm algorithm, int startIndex) {#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-}
```
public static void apply(List array, IAlgorithm algorithm, int startIndex)
```


Pas algoritme toe op elk lijstonderdeel beginnend vanaf de opgegeven positie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| array | java.util.List | ArrayList om te verwerken. |
| algoritme | com.aspose.tasks.IAlgorithm | Toegepast algoritme. |
| startIndex | int | Startpositie van het element. |

### filter(List array, ICondition cond) {#filter-java.util.List-com.aspose.tasks.ICondition-}
```
public static List filter(List array, ICondition cond)
```


Filter ArrayList-elementen op basis van de opgegeven voorwaarde.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| array | java.util.List | Lijst om te verwerken. |
| cond | com.aspose.tasks.ICondition | Voorwaarde gebruikt om de lijst te filteren. |

**Returns:**
java.util.List - Gefilterde lijst.
### find(List array, ICondition cond) {#find-java.util.List-com.aspose.tasks.ICondition-}
```
public static Object find(List array, ICondition cond)
```


Vind de eerste voorkoming van een ArrayList-element dat voldoet aan de opgegeven voorwaarde.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| array | java.util.List | ArrayList om te verwerken. |
| cond | com.aspose.tasks.ICondition | Voorwaarde gebruikt om een ArrayList-element te vinden. |

**Returns:**
java.lang.Object - Lijstonderdeel of null.
