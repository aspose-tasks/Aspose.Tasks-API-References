---
title: "ResourceCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta una raccolta di oggetti."
type: docs
weight: 251
url: /it/java/com.aspose.tasks/resourcecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceCollection extends AbstractList<Resource>
```

Rappresenta una collezione di oggetti [Resource](../../com.aspose.tasks/resource).
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add()](#add--) | Aggiunge una nuova risorsa all'ultima posizione della collezione di risorse di un progetto. |
| [add(Resource e)](#add-com.aspose.tasks.Resource-) | \{@inheritDoc\} |
| [add(String resourceName)](#add-java.lang.String-) | Aggiunge una nuova risorsa all'ultima posizione della collezione di risorse di un progetto. |
| [add(String resourceName, int beforeResourceId)](#add-java.lang.String-int-) | Aggiunge una nuova risorsa nella posizione specificata di una raccolta di risorse del progetto. |
| [clear()](#clear--) | La cancellazione diretta non è supportata, questo metodo lancia semplicemente UnsupportedOperationException. |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getById(int id)](#getById-int-) | Restituisce una risorsa con l'ID specificato. |
| [getByUid(int uid)](#getByUid-int-) | Restituisce una risorsa con l'Uid specificato. |
| [getParentProject()](#getParentProject--) | Ottiene il progetto genitore dell'oggetto ResourceCollection. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | \{@inheritDoc\} |
| [iterator()](#iterator--) | Restituisce un enumeratore per questa collezione. |
| [remove(Object o)](#remove-java.lang.Object-) | Questa è l'implementazione stub del metodo remove di Collection, che lancia solo UnsupportedOperationException |
| [size()](#size--) | Ottiene il numero di elementi contenuti nella ResourceCollection. |
| [sort(Comparator&lt;? super Resource&gt; comparer)](#sort-java.util.Comparator---super-com.aspose.tasks.Resource--) | \{@inheritDoc\} |
| [toList()](#toList--) | Converte l'oggetto ResourceCollection in un elenco di oggetti [Resource](../../com.aspose.tasks/resource). |
### add() {#add--}
```
public final Resource add()
```


Aggiunge una nuova risorsa all'ultima posizione della collezione di risorse di un progetto.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(Resource e) {#add-com.aspose.tasks.Resource-}
```
public final boolean add(Resource e)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| e | [Resource](../../com.aspose.tasks/resource) | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### add(String resourceName) {#add-java.lang.String-}
```
public final Resource add(String resourceName)
```


Aggiunge una nuova risorsa all'ultima posizione della collezione di risorse di un progetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| resourceName | java.lang.String | Nome di una risorsa. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(String resourceName, int beforeResourceId) {#add-java.lang.String-int-}
```
public final Resource add(String resourceName, int beforeResourceId)
```


Aggiunge una nuova risorsa nella posizione specificata di una raccolta di risorse del progetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| resourceName | java.lang.String | Nome di una risorsa. |
| beforeResourceId | int | Posizione della risorsa precedente in una raccolta di risorse del progetto. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### clear() {#clear--}
```
public final void clear()
```


La cancellazione diretta non è supportata, questo metodo lancia semplicemente UnsupportedOperationException.

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
public Resource get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Resource getById(int id)
```


Restituisce una risorsa con l'ID specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | id | int | L'ID specificato. |

--------------------

Complessità O(1). |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified id if present; otherwise, null.
### getByUid(int uid) {#getByUid-int-}
```
public final Resource getByUid(int uid)
```


Restituisce una risorsa con l'Uid specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | uid | int | L'uid specificato. |

--------------------

Complessità O(1). |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Ottiene il progetto genitore dell'oggetto ResourceCollection.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceCollection object.
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




**Returns:**
boolean - \{@inheritDoc\}
### iterator() {#iterator--}
```
public final Iterator<Resource> iterator()
```


Restituisce un enumeratore per questa collezione.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Resource&gt; - un enumeratore per questa raccolta.
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


Questa è l'implementazione stub del metodo remove di Collection, che lancia solo UnsupportedOperationException

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | l'elemento da rimuovere. |

**Returns:**
boolean - `true` se l'elemento è stato rimosso; `false` altrimenti.
### size() {#size--}
```
public final int size()
```


Ottiene il numero di elementi contenuti nella ResourceCollection.

--------------------

`int` di sola lettura.

**Returns:**
int - il numero di elementi contenuti nella ResourceCollection.
### sort(Comparator&lt;? super Resource&gt; comparer) {#sort-java.util.Comparator---super-com.aspose.tasks.Resource--}
```
public final void sort(Comparator<? super Resource> comparer)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| comparer | java.util.Comparator&lt;? super com.aspose.tasks.Resource&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<Resource> toList()
```


Converte l'oggetto ResourceCollection in un elenco di oggetti [Resource](../../com.aspose.tasks/resource).

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - elenco di oggetti [Resource](../../com.aspose.tasks/resource).
