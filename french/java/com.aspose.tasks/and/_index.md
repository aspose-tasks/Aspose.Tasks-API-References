---
title: "And"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Applique un ET logique aux conditions spécifiées."
type: docs
weight: 10
url: /fr/java/com.aspose.tasks/and/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class And<T> implements ICondition<T>
```

Applique un ET logique aux conditions spécifiées.

T : Le type d'objet auquel appliquer l'interface de méthode.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2)](#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--) | Initialise une nouvelle instance de la classe And&lt;T&gt;. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [check(T el)](#check-T-) | Renvoie vrai si l'objet spécifié satisfait les conditions. |
### And(ICondition&lt;T&gt; cond1, ICondition&lt;T&gt; cond2) {#And-com.aspose.tasks.ICondition-T--com.aspose.tasks.ICondition-T--}
```
public And(ICondition<T> cond1, ICondition<T> cond2)
```


Initialise une nouvelle instance de la classe And&lt;T&gt;.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cond1 | [ICondition](../../com.aspose.tasks/icondition) | Première condition. |
| cond2 | [ICondition](../../com.aspose.tasks/icondition) | Deuxième condition. |

### check(T el) {#check-T-}
```
public boolean check(T el)
```


Renvoie vrai si l'objet spécifié satisfait les conditions.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| el | T | L'objet à vérifier. |

**Returns:**
boolean - Vrai si l'objet satisfait les conditions.
