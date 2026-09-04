---
title: "RemoveTask"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Supprime la tâche spécifiée d'un arbre de tâches."
type: docs
weight: 246
url: /fr/java/com.aspose.tasks/removetask/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ITreeAlgorithm
```
public class RemoveTask implements ITreeAlgorithm<Task>
```

Supprime la tâche spécifiée d'un arbre de tâches.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [RemoveTask(Task task)](#RemoveTask-com.aspose.tasks.Task-) | Initialise une nouvelle instance de la classe [RemoveTask](../../com.aspose.tasks/removetask). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [alg(Task el, int level)](#alg-com.aspose.tasks.Task-int-) | Ne rien faire. |
| [postAlg(Task el, int level)](#postAlg-com.aspose.tasks.Task-int-) | Ne rien faire. |
| [preAlg(Task el, int level)](#preAlg-com.aspose.tasks.Task-int-) | Supprime la tâche du parent spécifié. |
### RemoveTask(Task task) {#RemoveTask-com.aspose.tasks.Task-}
```
public RemoveTask(Task task)
```


Initialise une nouvelle instance de la classe [RemoveTask](../../com.aspose.tasks/removetask).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Tâche à supprimer. |

### alg(Task el, int level) {#alg-com.aspose.tasks.Task-int-}
```
public final void alg(Task el, int level)
```


Ne rien faire.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Objet à traiter. |
| niveau | int | Niveau du nœud d'arbre. |

### postAlg(Task el, int level) {#postAlg-com.aspose.tasks.Task-int-}
```
public final void postAlg(Task el, int level)
```


Ne rien faire.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Objet à traiter. |
| niveau | int | Niveau du nœud d'arbre. |

### preAlg(Task el, int level) {#preAlg-com.aspose.tasks.Task-int-}
```
public final void preAlg(Task el, int level)
```


Supprime la tâche du parent spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Tâche parent. |
| niveau | int | Niveau du nœud d'arbre. |

