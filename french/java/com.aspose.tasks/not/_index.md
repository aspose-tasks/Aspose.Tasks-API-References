---
title: "Non"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Applique le NOT logique à la condition spécifiée."
type: docs
weight: 162
url: /fr/java/com.aspose.tasks/not/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class Not<T> implements ICondition<T>
```

Applique le NOT logique à la condition spécifiée.

T : Le type d'objet auquel appliquer l'interface de méthode.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Not(ICondition&lt;T&gt; condition)](#Not-com.aspose.tasks.ICondition-T--) | Initialise une nouvelle instance de la classe Not&lt;T&gt;. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [check(T el)](#check-T-) | Renvoie vrai si l'objet spécifié satisfait la condition. |
### Not(ICondition&lt;T&gt; condition) {#Not-com.aspose.tasks.ICondition-T--}
```
public Not(ICondition<T> condition)
```


Initialise une nouvelle instance de la classe Not&lt;T&gt;.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| condition | [ICondition](../../com.aspose.tasks/icondition) | Condition spécifiée. |

### check(T el) {#check-T-}
```
public boolean check(T el)
```


Renvoie vrai si l'objet spécifié satisfait la condition.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| el | T | L'objet à vérifier. |

**Returns:**
boolean - Vrai si l'objet satisfait la condition.
