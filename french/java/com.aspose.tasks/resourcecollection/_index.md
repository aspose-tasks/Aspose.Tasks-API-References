---
title: "ResourceCollection"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente une collection d'objets."
type: docs
weight: 251
url: /fr/java/com.aspose.tasks/resourcecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceCollection extends AbstractList<Resource>
```

Représente une collection d'objets [Resource](../../com.aspose.tasks/resource).
## Méthodes

| Méthode | Description |
| --- | --- |
| [add()](#add--) | Ajoute une nouvelle ressource à la dernière position d'une collection de ressources de projet. |
| [add(Resource e)](#add-com.aspose.tasks.Resource-) | \{@inheritDoc\} |
| [add(String resourceName)](#add-java.lang.String-) | Ajoute une nouvelle ressource à la dernière position d'une collection de ressources de projet. |
| [add(String resourceName, int beforeResourceId)](#add-java.lang.String-int-) | Ajoute une nouvelle ressource à la position spécifiée d’une collection de ressources de projet. |
| [clear()](#clear--) | Le nettoyage direct n’est pas pris en charge, cette méthode lève simplement une UnsupportedOperationException. |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getById(int id)](#getById-int-) | Renvoie une ressource avec l’identifiant spécifié. |
| [getByUid(int uid)](#getByUid-int-) | Renvoie une ressource avec l’Uid spécifié. |
| [getParentProject()](#getParentProject--) | Obtient le projet parent de l’objet ResourceCollection. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | \{@inheritDoc\} |
| [iterator()](#iterator--) | Renvoie un énumérateur pour cette collection. |
| [remove(Object o)](#remove-java.lang.Object-) | Ceci est l’implémentation factice de la méthode remove de Collection, qui ne fait que lever une UnsupportedOperationException |
| [size()](#size--) | Obtient le nombre d’éléments contenus dans le ResourceCollection. |
| [sort(Comparator&lt;? super Resource&gt; comparer)](#sort-java.util.Comparator---super-com.aspose.tasks.Resource--) | \{@inheritDoc\} |
| [toList()](#toList--) | Convertit l’objet ResourceCollection en une liste d’objets [Resource](../../com.aspose.tasks/resource). |
### add() {#add--}
```
public final Resource add()
```


Ajoute une nouvelle ressource à la dernière position d'une collection de ressources de projet.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(Resource e) {#add-com.aspose.tasks.Resource-}
```
public final boolean add(Resource e)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| e | [Resource](../../com.aspose.tasks/resource) | \{@inheritDoc\} |

**Returns:**
booléen - \{@inheritDoc\}
### add(String resourceName) {#add-java.lang.String-}
```
public final Resource add(String resourceName)
```


Ajoute une nouvelle ressource à la dernière position d'une collection de ressources de projet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| resourceName | java.lang.String | Nom d’une ressource. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(String resourceName, int beforeResourceId) {#add-java.lang.String-int-}
```
public final Resource add(String resourceName, int beforeResourceId)
```


Ajoute une nouvelle ressource à la position spécifiée d’une collection de ressources de projet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| resourceName | java.lang.String | Nom d’une ressource. |
| beforeResourceId | int | Position de la ressource précédente dans une collection de ressources de projet. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### clear() {#clear--}
```
public final void clear()
```


Le nettoyage direct n’est pas pris en charge, cette méthode lève simplement une UnsupportedOperationException.

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
public Resource get(int index)
```


(@inheritDoc\}

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| indice | int | \{@inheritDoc\} |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Resource getById(int id)
```


Renvoie une ressource avec l’identifiant spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | id | int | L’identifiant spécifié. |

--------------------

Complexité O(1). |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified id if present; otherwise, null.
### getByUid(int uid) {#getByUid-int-}
```
public final Resource getByUid(int uid)
```


Renvoie une ressource avec l’Uid spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | uid | int | L'uid spécifié. |

--------------------

Complexité O(1). |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Obtient le projet parent de l’objet ResourceCollection.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceCollection object.
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




**Returns:**
booléen - \{@inheritDoc\}
### iterator() {#iterator--}
```
public final Iterator<Resource> iterator()
```


Renvoie un énumérateur pour cette collection.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Resource&gt; - un itérateur pour cette collection.
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


Ceci est l’implémentation factice de la méthode remove de Collection, qui ne fait que lever une UnsupportedOperationException

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | l’élément à supprimer. |

**Returns:**
booléen - `true` si l'élément a été supprimé ; `false` sinon.
### size() {#size--}
```
public final int size()
```


Obtient le nombre d’éléments contenus dans le ResourceCollection.

--------------------

`int` en lecture seule.

**Returns:**
int - le nombre d’éléments contenus dans le ResourceCollection.
### sort(Comparator&lt;? super Resource&gt; comparer) {#sort-java.util.Comparator---super-com.aspose.tasks.Resource--}
```
public final void sort(Comparator<? super Resource> comparer)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| comparer | java.util.Comparator&lt;? super com.aspose.tasks.Resource&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<Resource> toList()
```


Convertit l’objet ResourceCollection en une liste d’objets [Resource](../../com.aspose.tasks/resource).

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - Liste d’objets [Resource](../../com.aspose.tasks/resource).
