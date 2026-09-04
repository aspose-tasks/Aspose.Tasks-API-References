---
title: "ResourceAssignmentCollection"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente une collection d'objets."
type: docs
weight: 250
url: /fr/java/com.aspose.tasks/resourceassignmentcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceAssignmentCollection extends AbstractList<ResourceAssignment>
```

Représente une collection d'objets [ResourceAssignment](../../com.aspose.tasks/resourceassignment).
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(ResourceAssignment item)](#add-com.aspose.tasks.ResourceAssignment-) | Ceci est l’implémentation factice de la méthode Add de ICollection, qui ne fait que lever UnsupportedOperationException. |
| [add(Task task, Resource resource)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-) | Ajoute une nouvelle affectation à la ResourceAssignmentCollection. |
| [add(Task task, Resource resource, double units)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-) | Ajoute une nouvelle affectation à la ResourceAssignmentCollection. |
| [add(Task task, Resource resource, BigDecimal cost)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-) | Ajoute une nouvelle affectation à la ResourceAssignmentCollection. |
| [clear()](#clear--) | Supprime tous les éléments de la collection. |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getByUid(int uid)](#getByUid-int-) | Renvoie une affectation avec l'uid spécifié. |
| [getParentProject()](#getParentProject--) | Obtient le projet parent de l'objet ResourceAssignmentCollection. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Obtient une valeur indiquant si cette collection est en lecture seule. |
| [iterator()](#iterator--) | Renvoie un énumérateur pour cette collection. |
| [remove(int index)](#remove-int-) | \{@inheritDoc\} |
| [remove(Object o)](#remove-java.lang.Object-) | Supprime l'affectation spécifiée de la collection, si elle n'est pas en lecture seule, sinon lève UnsupportedOperationException. |
| [size()](#size--) | Obtient le nombre d'objets contenus dans la ResourceAssignmentCollection. |
| [toList()](#toList--) | Convertit l'objet ResourceAssignmentCollection en une liste d'objets [ResourceAssignment](../../com.aspose.tasks/resourceassignment). |
### add(ResourceAssignment item) {#add-com.aspose.tasks.ResourceAssignment-}
```
public final boolean add(ResourceAssignment item)
```


Ceci est l’implémentation factice de la méthode Add de ICollection, qui ne fait que lever UnsupportedOperationException.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| item | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | L'élément à supprimer. |

**Returns:**
booléen - \{@inheritDoc\}
### add(Task task, Resource resource) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-}
```
public final ResourceAssignment add(Task task, Resource resource)
```


Ajoute une nouvelle affectation à la ResourceAssignmentCollection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Une tâche à affecter. |
| resource | [Resource](../../com.aspose.tasks/resource) | Une ressource à affecter. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, double units) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-}
```
public final ResourceAssignment add(Task task, Resource resource, double units)
```


Ajoute une nouvelle affectation à la ResourceAssignmentCollection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Une tâche à affecter. |
| resource | [Resource](../../com.aspose.tasks/resource) | Une ressource à affecter. |
| unités | double | Le nombre d'unités pour une nouvelle affectation. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, BigDecimal cost) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-}
```
public final ResourceAssignment add(Task task, Resource resource, BigDecimal cost)
```


Ajoute une nouvelle affectation à la ResourceAssignmentCollection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Une tâche à affecter. |
| resource | [Resource](../../com.aspose.tasks/resource) | Une ressource de coût à affecter. |
| coût | java.math.BigDecimal | Le coût pour une nouvelle affectation. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### clear() {#clear--}
```
public void clear()
```


Supprime tous les éléments de la collection.

### contains(Object o) {#contains-java.lang.Object-}
```
public final boolean contains(Object o)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
booléen - \{@inheritDoc\}
### get(int index) {#get-int-}
```
public ResourceAssignment get(int index)
```


(@inheritDoc\}

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| indice | int | \{@inheritDoc\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### getByUid(int uid) {#getByUid-int-}
```
public final ResourceAssignment getByUid(int uid)
```


Renvoie une affectation avec l'uid spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | uid | int | L'uid spécifié. |

--------------------

Complexité O(1). |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - ResourceAssignment with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Obtient le projet parent de l'objet ResourceAssignmentCollection.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceAssignmentCollection object.
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
public final Iterator<ResourceAssignment> iterator()
```


Renvoie un énumérateur pour cette collection.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.ResourceAssignment&gt; - un itérateur pour cette collection.
### remove(int index) {#remove-int-}
```
public ResourceAssignment remove(int index)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| indice | int | \{@inheritDoc\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


Supprime l'affectation spécifiée de la collection, si elle n'est pas en lecture seule, sinon lève UnsupportedOperationException.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | L'affectation à supprimer. |

**Returns:**
boolean - true, si l'élément spécifié a été supprimé, false sinon.
### size() {#size--}
```
public final int size()
```


Obtient le nombre d'objets contenus dans la ResourceAssignmentCollection.

**Returns:**
int - le nombre d'objets contenus dans le ResourceAssignmentCollection.
### toList() {#toList--}
```
public final List<ResourceAssignment> toList()
```


Convertit l'objet ResourceAssignmentCollection en une liste d'objets [ResourceAssignment](../../com.aspose.tasks/resourceassignment).

**Returns:**
java.util.List&lt;com.aspose.tasks.ResourceAssignment&gt; - Liste d'objets [ResourceAssignment](../../com.aspose.tasks/resourceassignment).
