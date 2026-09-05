---
title: "ResourceAssignmentCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta una raccolta di oggetti."
type: docs
weight: 250
url: /it/java/com.aspose.tasks/resourceassignmentcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceAssignmentCollection extends AbstractList<ResourceAssignment>
```

Rappresenta una collezione di oggetti [ResourceAssignment](../../com.aspose.tasks/resourceassignment).
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(ResourceAssignment item)](#add-com.aspose.tasks.ResourceAssignment-) | Questa è l'implementazione stub del metodo Add di ICollection, che lancia solo UnsupportedOperationException |
| [add(Task task, Resource resource)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-) | Aggiunge una nuova assegnazione alla ResourceAssignmentCollection. |
| [add(Task task, Resource resource, double units)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-) | Aggiunge una nuova assegnazione alla ResourceAssignmentCollection. |
| [add(Task task, Resource resource, BigDecimal cost)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-) | Aggiunge una nuova assegnazione alla ResourceAssignmentCollection. |
| [clear()](#clear--) | Rimuove tutti gli elementi dalla collezione. |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getByUid(int uid)](#getByUid-int-) | Restituisce un'assegnazione con l'uid specificato. |
| [getParentProject()](#getParentProject--) | Ottiene il progetto padre dell'oggetto ResourceAssignmentCollection. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Ottiene un valore che indica se questa collezione è di sola lettura. |
| [iterator()](#iterator--) | Restituisce un enumeratore per questa collezione. |
| [remove(int index)](#remove-int-) | \{@inheritDoc\} |
| [remove(Object o)](#remove-java.lang.Object-) | Rimuove l'assegnazione specificata dalla collezione, se non è di sola lettura, altrimenti genera UnsupportedOperationException. |
| [size()](#size--) | Ottiene il numero di oggetti contenuti nella ResourceAssignmentCollection. |
| [toList()](#toList--) | Converte l'oggetto ResourceAssignmentCollection in un elenco di oggetti [ResourceAssignment](../../com.aspose.tasks/resourceassignment). |
### add(ResourceAssignment item) {#add-com.aspose.tasks.ResourceAssignment-}
```
public final boolean add(ResourceAssignment item)
```


Questa è l'implementazione stub del metodo Add di ICollection, che lancia solo UnsupportedOperationException

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| item | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | L'elemento da rimuovere. |

**Returns:**
boolean - \{@inheritDoc\}
### add(Task task, Resource resource) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-}
```
public final ResourceAssignment add(Task task, Resource resource)
```


Aggiunge una nuova assegnazione alla ResourceAssignmentCollection.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Un'attività da assegnare. |
| resource | [Resource](../../com.aspose.tasks/resource) | Una risorsa da assegnare. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, double units) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-}
```
public final ResourceAssignment add(Task task, Resource resource, double units)
```


Aggiunge una nuova assegnazione alla ResourceAssignmentCollection.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Un'attività da assegnare. |
| resource | [Resource](../../com.aspose.tasks/resource) | Una risorsa da assegnare. |
| unità | double | Il numero di unità per una nuova assegnazione. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, BigDecimal cost) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-}
```
public final ResourceAssignment add(Task task, Resource resource, BigDecimal cost)
```


Aggiunge una nuova assegnazione alla ResourceAssignmentCollection.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Un'attività da assegnare. |
| resource | [Resource](../../com.aspose.tasks/resource) | Una risorsa di costo da assegnare. |
| costo | java.math.BigDecimal | Il costo per una nuova assegnazione. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### clear() {#clear--}
```
public void clear()
```


Rimuove tutti gli elementi dalla collezione.

### contains(Object o) {#contains-java.lang.Object-}
```
public final boolean contains(Object o)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### get(int index) {#get-int-}
```
public ResourceAssignment get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### getByUid(int uid) {#getByUid-int-}
```
public final ResourceAssignment getByUid(int uid)
```


Restituisce un'assegnazione con l'uid specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | uid | int | L'uid specificato. |

--------------------

Complessità O(1). |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - ResourceAssignment with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Ottiene il progetto padre dell'oggetto ResourceAssignmentCollection.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceAssignmentCollection object.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Ottiene un valore che indica se questa collezione è di sola lettura.

**Returns:**
boolean - un valore che indica se questa collezione è di sola lettura.
### iterator() {#iterator--}
```
public final Iterator<ResourceAssignment> iterator()
```


Restituisce un enumeratore per questa collezione.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.ResourceAssignment&gt; - un enumeratore per questa collezione.
### remove(int index) {#remove-int-}
```
public ResourceAssignment remove(int index)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


Rimuove l'assegnazione specificata dalla collezione, se non è di sola lettura, altrimenti genera UnsupportedOperationException.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | L'assegnazione da rimuovere. |

**Returns:**
boolean - true, se l'elemento specificato è stato rimosso, false altrimenti.
### size() {#size--}
```
public final int size()
```


Ottiene il numero di oggetti contenuti nella ResourceAssignmentCollection.

**Returns:**
int - il numero di oggetti contenuti nella ResourceAssignmentCollection.
### toList() {#toList--}
```
public final List<ResourceAssignment> toList()
```


Converte l'oggetto ResourceAssignmentCollection in un elenco di oggetti [ResourceAssignment](../../com.aspose.tasks/resourceassignment).

**Returns:**
java.util.List&lt;com.aspose.tasks.ResourceAssignment&gt; - Elenco di oggetti [ResourceAssignment](../../com.aspose.tasks/resourceassignment).
