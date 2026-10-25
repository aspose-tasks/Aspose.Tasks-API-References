---
title: "ResourceAssignmentCollection"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa una colección de objetos."
type: docs
weight: 250
url: /es/java/com.aspose.tasks/resourceassignmentcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceAssignmentCollection extends AbstractList<ResourceAssignment>
```

Representa una colección de objetos [ResourceAssignment](../../com.aspose.tasks/resourceassignment).
## Métodos

| Método | Descripción |
| --- | --- |
| [add(ResourceAssignment item)](#add-com.aspose.tasks.ResourceAssignment-) | Esta es la implementación de sustituto del método Add de ICollection, que solo lanza UnsupportedOperationException |
| [add(Task task, Resource resource)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-) | Agrega una nueva asignación a la ResourceAssignmentCollection. |
| [add(Task task, Resource resource, double units)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-) | Agrega una nueva asignación a la ResourceAssignmentCollection. |
| [add(Task task, Resource resource, BigDecimal cost)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-) | Agrega una nueva asignación a la ResourceAssignmentCollection. |
| [clear()](#clear--) | Elimina todos los elementos de la colección. |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getByUid(int uid)](#getByUid-int-) | Devuelve una asignación con el uid especificado. |
| [getParentProject()](#getParentProject--) | Obtiene el proyecto padre del objeto ResourceAssignmentCollection. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Obtiene un valor que indica si esta colección es de solo lectura. |
| [iterator()](#iterator--) | Devuelve un enumerador para esta colección. |
| [remove(int index)](#remove-int-) | \{@inheritDoc\} |
| [remove(Object o)](#remove-java.lang.Object-) | Elimina la asignación especificada de la colección, si no es de solo lectura; de lo contrario lanza UnsupportedOperationException. |
| [size()](#size--) | Obtiene el número de objetos contenidos en la ResourceAssignmentCollection. |
| [toList()](#toList--) | Convierte el objeto ResourceAssignmentCollection a una lista de objetos [ResourceAssignment](../../com.aspose.tasks/resourceassignment). |
### add(ResourceAssignment item) {#add-com.aspose.tasks.ResourceAssignment-}
```
public final boolean add(ResourceAssignment item)
```


Esta es la implementación de sustituto del método Add de ICollection, que solo lanza UnsupportedOperationException

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| item | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | El elemento a eliminar. |

**Returns:**
boolean - \{@inheritDoc\}
### add(Task task, Resource resource) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-}
```
public final ResourceAssignment add(Task task, Resource resource)
```


Agrega una nueva asignación a la ResourceAssignmentCollection.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Una tarea a asignar. |
| resource | [Resource](../../com.aspose.tasks/resource) | Un recurso a asignar. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, double units) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-}
```
public final ResourceAssignment add(Task task, Resource resource, double units)
```


Agrega una nueva asignación a la ResourceAssignmentCollection.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Una tarea a asignar. |
| resource | [Resource](../../com.aspose.tasks/resource) | Un recurso a asignar. |
| unidades | double | El número de unidades para una nueva asignación. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, BigDecimal cost) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-}
```
public final ResourceAssignment add(Task task, Resource resource, BigDecimal cost)
```


Agrega una nueva asignación a la ResourceAssignmentCollection.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Una tarea a asignar. |
| resource | [Resource](../../com.aspose.tasks/resource) | Un recurso de costo a asignar. |
| costo | java.math.BigDecimal | El costo para una nueva asignación. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### clear() {#clear--}
```
public void clear()
```


Elimina todos los elementos de la colección.

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
public ResourceAssignment get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | \{@inheritDoc\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### getByUid(int uid) {#getByUid-int-}
```
public final ResourceAssignment getByUid(int uid)
```


Devuelve una asignación con el uid especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | uid | int | El uid especificado. |

--------------------

Complejidad O(1). |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - ResourceAssignment with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Obtiene el proyecto padre del objeto ResourceAssignmentCollection.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceAssignmentCollection object.
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


Obtiene un valor que indica si esta colección es de solo lectura.

**Returns:**
boolean - un valor que indica si esta colección es de solo lectura.
### iterator() {#iterator--}
```
public final Iterator<ResourceAssignment> iterator()
```


Devuelve un enumerador para esta colección.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.ResourceAssignment&gt; - un enumerador para esta colección.
### remove(int index) {#remove-int-}
```
public ResourceAssignment remove(int index)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | \{@inheritDoc\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


Elimina la asignación especificada de la colección, si no es de solo lectura; de lo contrario lanza UnsupportedOperationException.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | java.lang.Object | La asignación a eliminar. |

**Returns:**
boolean - true, si el elemento especificado fue eliminado, false en caso contrario.
### size() {#size--}
```
public final int size()
```


Obtiene el número de objetos contenidos en la ResourceAssignmentCollection.

**Returns:**
int - el número de objetos contenidos en la ResourceAssignmentCollection.
### toList() {#toList--}
```
public final List<ResourceAssignment> toList()
```


Convierte el objeto ResourceAssignmentCollection a una lista de objetos [ResourceAssignment](../../com.aspose.tasks/resourceassignment).

**Returns:**
java.util.List&lt;com.aspose.tasks.ResourceAssignment&gt; - Lista de objetos [ResourceAssignment](../../com.aspose.tasks/resourceassignment).
