---
title: "ArrayUtils"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Classe utilitaire pour le traitement d'ArrayList."
type: docs
weight: 14
url: /fr/java/com.aspose.tasks/arrayutils/
---

**Inheritance:**
java.lang.Object
```
public class ArrayUtils
```

Classe utilitaire pour le traitement d'ArrayList.
## Méthodes

| Méthode | Description |
| --- | --- |
| [&lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[][] arrays)](#-T-concat-java.lang.Class-T--T--...-) |  |
| [apply(List array, IAlgorithm algorithm, int startIndex)](#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-) | Appliquer l'algorithme à chaque élément de la liste à partir de la position spécifiée. |
| [filter(List array, ICondition cond)](#filter-java.util.List-com.aspose.tasks.ICondition-) | Filtrer les éléments d'ArrayList selon la condition spécifiée. |
| [find(List array, ICondition cond)](#find-java.util.List-com.aspose.tasks.ICondition-) | Trouver la première occurrence d'un élément d'ArrayList qui satisfait la condition spécifiée. |
### &lt;T&gt;concat(Class&lt;T&gt; typeOfT, T[][] arrays) {#-T-concat-java.lang.Class-T--T--...-}
```
public static T[] <T>concat(Class<T> typeOfT, T[][] arrays)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| typeOfT | java.lang.Class&lt;T&gt; |  |
| tableaux | T[][] |  |

**Returns:**
T[]
### apply(List array, IAlgorithm algorithm, int startIndex) {#apply-java.util.List-com.aspose.tasks.IAlgorithm-int-}
```
public static void apply(List array, IAlgorithm algorithm, int startIndex)
```


Appliquer l'algorithme à chaque élément de la liste à partir de la position spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| tableau | java.util.List | ArrayList à traiter. |
| algorithme | com.aspose.tasks.IAlgorithm | Algorithme appliqué. |
| startIndex | int | Position de l'élément de départ. |

### filter(List array, ICondition cond) {#filter-java.util.List-com.aspose.tasks.ICondition-}
```
public static List filter(List array, ICondition cond)
```


Filtrer les éléments d'ArrayList selon la condition spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| tableau | java.util.List | Liste à traiter. |
| cond | com.aspose.tasks.ICondition | Condition utilisée pour filtrer la liste. |

**Returns:**
java.util.List - Liste filtrée.
### find(List array, ICondition cond) {#find-java.util.List-com.aspose.tasks.ICondition-}
```
public static Object find(List array, ICondition cond)
```


Trouver la première occurrence d'un élément d'ArrayList qui satisfait la condition spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| tableau | java.util.List | ArrayList à traiter. |
| cond | com.aspose.tasks.ICondition | Condition utilisée pour trouver l'élément d'ArrayList. |

**Returns:**
java.lang.Object - Élément de liste ou null.
