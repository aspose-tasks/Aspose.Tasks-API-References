---
title: "TaskLinkCollection"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente une collection d'objets."
type: docs
weight: 296
url: /fr/java/com.aspose.tasks/tasklinkcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskLinkCollection extends AbstractList<TaskLink>
```

Représente une collection d'objets [Task](../../com.aspose.tasks/task).
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(Task pred, Task succ)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-) | Renvoie une instance de Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) qui a été ajoutée à l'objet TaskLinkCollection. |
| [add(Task pred, Task succ, int linkType)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-) | Renvoie une instance de [TaskLink](../../com.aspose.tasks/tasklink) qui a été ajoutée à l'objet TaskLinkCollection. |
| [add(Task pred, Task succ, int linkType, Duration lag)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-) | Renvoie une instance de [TaskLink](../../com.aspose.tasks/tasklink) qui a été ajoutée à l'objet TaskLinkCollection. |
| [add(TaskLink e)](#add-com.aspose.tasks.TaskLink-) | Ceci est l’implémentation factice de la méthode Add de ICollection, qui ne fait que lever UnsupportedOperationException. |
| [clear()](#clear--) | Réservé à un usage interne. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getParentProject()](#getParentProject--) | Obtient le projet parent de l'objet ResourceAssignmentCollection. |
| [remove(int index)](#remove-int-) | Supprime l'élément à la position spécifiée dans cette collection et renvoie l'élément qui a été supprimé de la collection. |
| [remove(Object item)](#remove-java.lang.Object-) | Supprime le lien de tâche d'un projet. |
| [size()](#size--) | Renvoie le nombre d'objets contenus dans cet objet `TaskLinkCollection`. |
| [sort(Comparator&lt;? super TaskLink&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--) | \{@inheritDoc\} |
| [toList()](#toList--) | Convertit l'objet TaskLinkCollection en une liste d'objets [TaskLink](../../com.aspose.tasks/tasklink). |
### add(Task pred, Task succ) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-}
```
public final TaskLink add(Task pred, Task succ)
```


Renvoie une instance de Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) qui a été ajoutée à l'objet TaskLinkCollection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Tâche prédécesseur. |
| succ | [Task](../../com.aspose.tasks/task) | Tâche successeur. |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-}
```
public final TaskLink add(Task pred, Task succ, int linkType)
```


Renvoie une instance de [TaskLink](../../com.aspose.tasks/tasklink) qui a été ajoutée à l'objet TaskLinkCollection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Tâche prédécesseur. |
| succ | [Task](../../com.aspose.tasks/task) | Tâche successeur. |
| linkType | int | Type de lien [TaskLinkType](../../com.aspose.tasks/tasklinktype) |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType, Duration lag) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-}
```
public final TaskLink add(Task pred, Task succ, int linkType, Duration lag)
```


Renvoie une instance de [TaskLink](../../com.aspose.tasks/tasklink) qui a été ajoutée à l'objet TaskLinkCollection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Tâche prédécesseur. |
| succ | [Task](../../com.aspose.tasks/task) | Tâche successeur. |
| linkType | int | Type de lien [TaskLinkType](../../com.aspose.tasks/tasklinktype) |
| lag | [Duration](../../com.aspose.tasks/duration) | Délai du lien [Duration](../../com.aspose.tasks/duration). |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link which has been added to this object.
### add(TaskLink e) {#add-com.aspose.tasks.TaskLink-}
```
public final boolean add(TaskLink e)
```


Ceci est l’implémentation factice de la méthode Add de ICollection, qui ne fait que lever UnsupportedOperationException.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| e | [TaskLink](../../com.aspose.tasks/tasklink) | L’élément à ajouter. |

**Returns:**
booléen - \{@inheritDoc\}
### clear() {#clear--}
```
public final void clear()
```


Réservé à un usage interne.

### get(int index) {#get-int-}
```
public TaskLink get(int index)
```


(@inheritDoc\}

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| indice | int | \{@inheritDoc\} |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - \{@inheritDoc\}
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Obtient le projet parent de l'objet ResourceAssignmentCollection.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent `Project` for this object.
### remove(int index) {#remove-int-}
```
public final TaskLink remove(int index)
```


Supprime l'élément à la position spécifiée dans cette collection et renvoie l'élément qui a été supprimé de la collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| indice | int | la position spécifiée pour supprimer l'élément. |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - the element that was removed from the collection.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


Supprime le lien de tâche d'un projet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| élément | java.lang.Object | l'instance spécifiée de la classe `TaskLink` à supprimer. |

**Returns:**
booléen - renvoie l'instance de la classe `TaskLink` qui a été supprimée de cette collection.
### size() {#size--}
```
public final int size()
```


Renvoie le nombre d'objets contenus dans cet objet `TaskLinkCollection`. Lecture seule `int`.

**Returns:**
int - renvoie le nombre d'objets contenus dans cette collection.
### sort(Comparator&lt;? super TaskLink&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--}
```
public void sort(Comparator<? super TaskLink> c)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| c | java.util.Comparator&lt;? super com.aspose.tasks.TaskLink&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<TaskLink> toList()
```


Convertit l'objet TaskLinkCollection en une liste d'objets [TaskLink](../../com.aspose.tasks/tasklink).

**Returns:**
java.util.List&lt;com.aspose.tasks.TaskLink&gt; - Liste d'objets [TaskLink](../../com.aspose.tasks/tasklink).
