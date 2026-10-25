---
title: "ChildTasksCollector"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Collecte toutes les sous‑tâches."
type: docs
weight: 49
url: /fr/java/com.aspose.tasks/childtaskscollector/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.TreeAlgorithmBase
```
public class ChildTasksCollector extends TreeAlgorithmBase<Task>
```

Collecte toutes les sous‑tâches.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ChildTasksCollector()](#ChildTasksCollector--) | Initialise une nouvelle instance de la classe [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [alg(Task el, int level)](#alg-com.aspose.tasks.Task-int-) | Traite l'objet spécifié. |
| [getTasks()](#getTasks--) | Obtient une liste d'objets enfants collectés (tâches). |
### ChildTasksCollector() {#ChildTasksCollector--}
```
public ChildTasksCollector()
```


Initialise une nouvelle instance de la classe [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector).

### alg(Task el, int level) {#alg-com.aspose.tasks.Task-int-}
```
public void alg(Task el, int level)
```


Traite l'objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Objet à traiter. |
| niveau | int | Niveau du nœud d'arbre. |

### getTasks() {#getTasks--}
```
public final List<Task> getTasks()
```


Obtient une liste d'objets enfants collectés (tâches).

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - une liste d'objets enfants collectés (tâches).
