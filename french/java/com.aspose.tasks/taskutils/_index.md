---
title: "TaskUtils"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Classe d'assistance qui fournit des opérations utiles avec les tâches."
type: docs
weight: 307
url: /fr/java/com.aspose.tasks/taskutils/
---

**Inheritance:**
java.lang.Object
```
public class TaskUtils
```

Classe d'assistance qui fournit des opérations utiles avec les tâches.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [TaskUtils()](#TaskUtils--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level)](#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-) | Applique l'algorithme spécifié à chaque tâche d'un arbre. |
| [filter(Task root, ICondition&lt;Task&gt; cond)](#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Construit un nouvel arbre de tâches qui satisfont la condition. |
| [find(Task root, ICondition&lt;Task&gt; cond)](#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Trouve une tâche qui satisfait la condition dans un arbre de tâches. |
| [taskChildrenCount(Task task)](#taskChildrenCount-com.aspose.tasks.Task-) | Calcule récursivement le nombre de sous‑tâches d'une tâche à travers tous les niveaux. |
### TaskUtils() {#TaskUtils--}
```
public TaskUtils()
```


### apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level) {#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-}
```
public static void apply(Task root, ITreeAlgorithm<Task> alg, int level)
```


Applique l'algorithme spécifié à chaque tâche d'un arbre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Racine de l'arbre |
| alg | com.aspose.tasks.ITreeAlgorithm&lt;com.aspose.tasks.Task&gt; | Algorithme appliqué. |
| niveau | int | Niveau de la tâche racine. |

### filter(Task root, ICondition&lt;Task&gt; cond) {#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task filter(Task root, ICondition<Task> cond)
```


Construit un nouvel arbre de tâches qui satisfont la condition.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Racine de l'arbre. |
| cond | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | Condition appliquée. |

**Returns:**
[Task](../../com.aspose.tasks/task) - Root of a new tree.
### find(Task root, ICondition&lt;Task&gt; cond) {#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task find(Task root, ICondition<Task> cond)
```


Trouve une tâche qui satisfait la condition dans un arbre de tâches.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Racine de l'arbre. |
| cond | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | Condition appliquée. |

**Returns:**
[Task](../../com.aspose.tasks/task) - Task if task was found, otherwise null.
### taskChildrenCount(Task task) {#taskChildrenCount-com.aspose.tasks.Task-}
```
public static int taskChildrenCount(Task task)
```


Calcule récursivement le nombre de sous‑tâches d'une tâche à travers tous les niveaux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | La tâche dont les enfants sont calculés. |

**Returns:**
int - Le nombre d'enfants.
