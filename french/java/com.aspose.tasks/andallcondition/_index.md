---
title: "AndAllCondition"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Applique un ET logique à toutes les conditions."
type: docs
weight: 11
url: /fr/java/com.aspose.tasks/andallcondition/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ICondition
```
public class AndAllCondition<T> implements ICondition<T>
```

Applique le ET logique à toutes les conditions. Par exemple : cond1 AND cond2 AND cond3...

T : Le type d'objet auquel appliquer l'interface de méthode.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions)](#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---) | Initialise une nouvelle instance de la classe AndAllCondition&lt;T&gt;. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [check(T el)](#check-T-) | Renvoie vrai si l'objet spécifié satisfait les conditions. |
### AndAllCondition(List&lt;ICondition&lt;T&gt;&gt; conditions) {#AndAllCondition-java.util.List-com.aspose.tasks.ICondition-T---}
```
public AndAllCondition(List<ICondition<T>> conditions)
```


Initialise une nouvelle instance de la classe AndAllCondition&lt;T&gt;.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| conditions | java.util.List&lt;com.aspose.tasks.ICondition&lt;T&gt;&gt; | La liste des conditions. |

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
