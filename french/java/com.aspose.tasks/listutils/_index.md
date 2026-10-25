---
title: "ListUtils"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Classe utilitaire pour le traitement des listes."
type: docs
weight: 147
url: /fr/java/com.aspose.tasks/listutils/
---

**Inheritance:**
java.lang.Object
```
public class ListUtils
```

Classe utilitaire pour le traitement des listes.
## Méthodes

| Méthode | Description |
| --- | --- |
| [&lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex)](#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-) | Appliquer l'algorithme à chaque élément de la liste à partir de la position spécifiée. |
| [&lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond)](#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--) | Filtrer les éléments de la liste selon la condition spécifiée. |
| [&lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz)](#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-) | Trouver la première occurrence d'un élément de liste qui satisfait la condition spécifiée. |
### &lt;T&gt;apply(List&lt;T&gt; list, IAlgorithm&lt;T&gt; algorithm, int startIndex) {#-T-apply-java.util.List-T--com.aspose.tasks.IAlgorithm-T--int-}
```
public static void <T>apply(List<T> list, IAlgorithm<T> algorithm, int startIndex)
```


Appliquer l'algorithme à chaque élément de la liste à partir de la position spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| liste | java.util.List&lt;T&gt; | Liste à traiter. |
| algorithm | [IAlgorithm](../../com.aspose.tasks/ialgorithm) | Algorithme appliqué. |
| startIndex | int | Position de l'élément de départ. |

### &lt;T&gt;filter(List&lt;T&gt; list, ICondition&lt;T&gt; cond) {#-T-filter-java.util.List-T--com.aspose.tasks.ICondition-T--}
```
public static List<T> <T>filter(List<T> list, ICondition<T> cond)
```


Filtrer les éléments de la liste selon la condition spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| liste | java.util.List&lt;T&gt; | Une liste à traiter. |
| cond | [ICondition](../../com.aspose.tasks/icondition) | Condition utilisée pour filtrer la liste spécifiée. |

**Returns:**
java.util.List&lt;T&gt; - Liste filtrée.
### &lt;T&gt;find(List&lt;T&gt; list, ICondition&lt;T&gt; cond, Class clazz) {#-T-find-java.util.List-T--com.aspose.tasks.ICondition-T--java.lang.Class-}
```
public static T <T>find(List<T> list, ICondition<T> cond, Class clazz)
```


Trouver la première occurrence d'un élément de liste qui satisfait la condition spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| liste | java.util.List&lt;T&gt; | Une liste à traiter. |
| cond | [ICondition](../../com.aspose.tasks/icondition) | Condition utilisée pour trouver un élément dans la liste spécifiée. |
| clazz | java.lang.Class | Type de classe de l'élément T. |

**Returns:**
T - Élément de liste ou null.
