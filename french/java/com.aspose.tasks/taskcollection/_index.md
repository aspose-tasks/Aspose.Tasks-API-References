---
title: "TaskCollection"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente une collection d'objets."
type: docs
weight: 293
url: /fr/java/com.aspose.tasks/taskcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskCollection extends AbstractList<Task>
```

Représente une collection d'objets [Task](../../com.aspose.tasks/task).
## Méthodes

| Méthode | Description |
| --- | --- |
| [add()](#add--) | Ajoute une nouvelle tâche à la collection des tâches du projet au même niveau hiérarchique que la dernière tâche. |
| [add(RecurringTaskParameters parameters)](#add-com.aspose.tasks.RecurringTaskParameters-) | Insère une nouvelle tâche avant une tâche avec l'identifiant spécifié et au même niveau hiérarchique. |
| [add(Task item)](#add-com.aspose.tasks.Task-) | Ajoute la tâche spécifiée à l'instance de la classe [TaskCollection](../../com.aspose.tasks/taskcollection). |
| [add(String taskName)](#add-java.lang.String-) | Ajoute une nouvelle tâche à la collection des tâches enfants. |
| [add(String taskName, int beforeTaskId)](#add-java.lang.String-int-) | Ajoute une nouvelle tâche récurrente à la collection des tâches enfants. |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Task item)](#contains-com.aspose.tasks.Task-) | Vérifie si la collection contient l'élément spécifié. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getById(int id)](#getById-int-) | Renvoie une tâche avec l'Id spécifié dont l'ancêtre est la tâche parent de cette collection. |
| [getByUid(int uid)](#getByUid-int-) | Renvoie une tâche avec le Uid spécifié dont l'ancêtre est la tâche parent de cette collection. |
| [getParentProject()](#getParentProject--) | Obtient le projet parent de l'objet TaskCollection. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Obtient une valeur indiquant si cette collection est en lecture seule. |
| [iterator()](#iterator--) | Renvoie un énumérateur pour cette collection. |
| [remove(Object item)](#remove-java.lang.Object-) | Ceci est l'implémentation factice de la méthode Remove de ICollection, qui ne lance que UnsupportedOperationException |
| [size()](#size--) | Obtient le nombre d'objets contenus dans le TaskCollection. |
| [sort(Comparator&lt;? super Task&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.Task--) | \{@inheritDoc\} |
| [toList()](#toList--) | Convertit l'objet TaskCollection en une liste d'objets [Task](../../com.aspose.tasks/task). |
### add() {#add--}
```
public final Task add()
```


Ajoute une nouvelle tâche à la collection des tâches du projet au même niveau hiérarchique que la dernière tâche.

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(RecurringTaskParameters parameters) {#add-com.aspose.tasks.RecurringTaskParameters-}
```
public final Task add(RecurringTaskParameters parameters)
```


Insère une nouvelle tâche avant une tâche avec l'identifiant spécifié et au même niveau hiérarchique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| parameters | [RecurringTaskParameters](../../com.aspose.tasks/recurringtaskparameters) | Les paramètres spécifiés pour la création d'une tâche récurrente. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(Task item) {#add-com.aspose.tasks.Task-}
```
public final boolean add(Task item)
```


Ajoutez la tâche spécifiée à l'instance de la classe [TaskCollection](../../com.aspose.tasks/taskcollection). Si ParentProject.CalculationMode est None, l'utilisateur doit appeler Project.Recalculate() après avoir utilisé cette méthode (Cela replanifiera toutes les tâches du projet (dates de début/fin, définit les dates anticipées/retardées) et calculera les champs dépendants tels que les marges, le travail et les champs de coût, les identifiants et les niveaux de hiérarchie). Si ParentProject.CalculationMode est Manual, la méthode calculera uniquement l'identifiant de la tâche, le niveau de hiérarchie et les numéros de hiérarchie automatiquement. Si ParentProject.CalculationMode est Automatic, la méthode replanifie automatiquement toutes les tâches du projet (dates de début/fin, définit les dates anticipées/retardées, calcule les marges, le travail et les champs de coût, recalcule les identifiants et les niveaux de hiérarchie).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | la tâche spécifiée qui doit être ajoutée à cette collection de tâches. |

**Returns:**
booléen - vrai si l'opération a réussi.
### add(String taskName) {#add-java.lang.String-}
```
public final Task add(String taskName)
```


Ajoute une nouvelle tâche à la collection des tâches enfants.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| taskName | java.lang.String | le nom de la tâche spécifiée. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(String taskName, int beforeTaskId) {#add-java.lang.String-int-}
```
public final Task add(String taskName, int beforeTaskId)
```


Ajoute une nouvelle tâche récurrente à la collection des tâches enfants.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| taskName | java.lang.String | le nom de la tâche spécifiée. |
| beforeTaskId | int | L'identifiant spécifié d'une tâche avant laquelle une nouvelle tâche sera insérée. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns a task which was inserted before a task with the specified id.
### clear() {#clear--}
```
public final void clear()
```




### contains(Task item) {#contains-com.aspose.tasks.Task-}
```
public final boolean contains(Task item)
```


Vérifie si la collection contient l'élément spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | L'élément à vérifier. |

**Returns:**
booléen - true, si la collection contient un élément, false sinon.
### get(int index) {#get-int-}
```
public Task get(int index)
```


(@inheritDoc\}

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| indice | int | \{@inheritDoc\} |

**Returns:**
[Task](../../com.aspose.tasks/task) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Task getById(int id)
```


Renvoie une tâche avec l'Id spécifié dont l'ancêtre est la tâche parent de cette collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| id | int | TaskEntity Id |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified id whose ancestor is parent task of this collection.
### getByUid(int uid) {#getByUid-int-}
```
public final Task getByUid(int uid)
```


Renvoie une tâche avec le Uid spécifié dont l'ancêtre est la tâche parent de cette collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| uid | int | TaskEntity Uid. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified uid whose ancestor is parent task of this collection.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Obtient le projet parent de l'objet TaskCollection.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the TaskCollection object.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Obtient une valeur indiquant si cette collection est en lecture seule.

**Returns:**
boolean - une valeur indiquant si cette collection est en lecture seule.
### iterator() {#iterator--}
```
public final Iterator<Task> iterator()
```


Renvoie un énumérateur pour cette collection.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Task&gt; - un itérateur pour cette collection.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


Ceci est l'implémentation factice de la méthode Remove de ICollection, qui ne lance que UnsupportedOperationException

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| élément | java.lang.Object | L'élément à supprimer. |

**Returns:**
booléen - `true` si l'élément a été supprimé ; `false` sinon.
### size() {#size--}
```
public final int size()
```


Obtient le nombre d'objets contenus dans le TaskCollection.

**Returns:**
int - le nombre d'objets contenus dans le TaskCollection.
### sort(Comparator&lt;? super Task&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.Task--}
```
public final void sort(Comparator<? super Task> c)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| c | java.util.Comparator&lt;? super com.aspose.tasks.Task&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<Task> toList()
```


Convertit l'objet TaskCollection en une liste d'objets [Task](../../com.aspose.tasks/task).

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - renvoie une liste qui contient les instances de la classe [Task](../../com.aspose.tasks/task) de cette collection.
