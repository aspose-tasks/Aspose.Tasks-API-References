---
title: "ResourceCollection"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa una colección de objetos."
type: docs
weight: 251
url: /es/java/com.aspose.tasks/resourcecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceCollection extends AbstractList<Resource>
```

Representa una colección de objetos [Resource](../../com.aspose.tasks/resource).
## Métodos

| Método | Descripción |
| --- | --- |
| [add()](#add--) | Agrega un nuevo recurso en la última posición de la colección de recursos de un proyecto. |
| [add(Resource e)](#add-com.aspose.tasks.Resource-) | \{@inheritDoc\} |
| [add(String resourceName)](#add-java.lang.String-) | Agrega un nuevo recurso en la última posición de la colección de recursos de un proyecto. |
| [add(String resourceName, int beforeResourceId)](#add-java.lang.String-int-) | Agrega un nuevo recurso en la posición especificada de una colección de recursos del proyecto. |
| [clear()](#clear--) | La eliminación directa no está soportada, este método solo lanza UnsupportedOperationException. |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getById(int id)](#getById-int-) | Devuelve un recurso con el id especificado. |
| [getByUid(int uid)](#getByUid-int-) | Devuelve un recurso con el Uid especificado. |
| [getParentProject()](#getParentProject--) | Obtiene el proyecto padre del objeto ResourceCollection. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | \{@inheritDoc\} |
| [iterator()](#iterator--) | Devuelve un enumerador para esta colección. |
| [remove(Object o)](#remove-java.lang.Object-) | Esta es la implementación de sustituto del método remove de Collection, que solo lanza UnsupportedOperationException |
| [size()](#size--) | Obtiene el número de elementos contenidos en el ResourceCollection. |
| [sort(Comparator&lt;? super Resource&gt; comparer)](#sort-java.util.Comparator---super-com.aspose.tasks.Resource--) | \{@inheritDoc\} |
| [toList()](#toList--) | Convierte el objeto ResourceCollection en una lista de objetos [Resource](../../com.aspose.tasks/resource). |
### add() {#add--}
```
public final Resource add()
```


Agrega un nuevo recurso en la última posición de la colección de recursos de un proyecto.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(Resource e) {#add-com.aspose.tasks.Resource-}
```
public final boolean add(Resource e)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| e | [Resource](../../com.aspose.tasks/resource) | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### add(String resourceName) {#add-java.lang.String-}
```
public final Resource add(String resourceName)
```


Agrega un nuevo recurso en la última posición de la colección de recursos de un proyecto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| resourceName | java.lang.String | Nombre de un recurso. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(String resourceName, int beforeResourceId) {#add-java.lang.String-int-}
```
public final Resource add(String resourceName, int beforeResourceId)
```


Agrega un nuevo recurso en la posición especificada de una colección de recursos del proyecto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| resourceName | java.lang.String | Nombre de un recurso. |
| beforeResourceId | int | Posición del recurso anterior en una colección de recursos del proyecto. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### clear() {#clear--}
```
public final void clear()
```


La eliminación directa no está soportada, este método solo lanza UnsupportedOperationException.

### contains(Object o) {#contains-java.lang.Object-}
```
public final boolean contains(Object o)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | \{@inheritDoc\} |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Resource getById(int id)
```


Devuelve un recurso con el id especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | id | int | El id especificado. |

--------------------

Complejidad O(1). |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified id if present; otherwise, null.
### getByUid(int uid) {#getByUid-int-}
```
public final Resource getByUid(int uid)
```


Devuelve un recurso con el Uid especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | uid | int | El uid especificado. |

--------------------

Complejidad O(1). |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Obtiene el proyecto padre del objeto ResourceCollection.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceCollection object.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
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


Devuelve un enumerador para esta colección.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Resource&gt; - un enumerador para esta colección.
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


Esta es la implementación de sustituto del método remove de Collection, que solo lanza UnsupportedOperationException

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | el elemento a eliminar. |

**Returns:**
boolean - `true` si el elemento fue eliminado; `false` de lo contrario.
### size() {#size--}
```
public final int size()
```


Obtiene el número de elementos contenidos en el ResourceCollection.

--------------------

Solo lectura `int`.

**Returns:**
int - el número de elementos contenidos en el ResourceCollection.
### sort(Comparator&lt;? super Resource&gt; comparer) {#sort-java.util.Comparator---super-com.aspose.tasks.Resource--}
```
public final void sort(Comparator<? super Resource> comparer)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| comparer | java.util.Comparator&lt;? super com.aspose.tasks.Resource&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<Resource> toList()
```


Convierte el objeto ResourceCollection en una lista de objetos [Resource](../../com.aspose.tasks/resource).

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - Lista de objetos [Resource](../../com.aspose.tasks/resource).
