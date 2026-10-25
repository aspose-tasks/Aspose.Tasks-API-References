---
title: "ViewCollection"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Contiene una lista de objetos."
type: docs
weight: 343
url: /es/java/com.aspose.tasks/viewcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class ViewCollection extends AbstractCollection<View>
```

Contiene una lista de objetos [View](../../com.aspose.tasks/view). Extiende la clase `AbstractCollection`.
## Métodos

| Método | Descripción |
| --- | --- |
| [add(View item)](#add-com.aspose.tasks.View-) | Agrega el elemento especificado a esta colección. |
| [clear()](#clear--) | Elimina todos los elementos de esta colección. |
| [contains(View item)](#contains-com.aspose.tasks.View-) | Devuelve true si el elemento especificado se encuentra en esta colección; de lo contrario, false. |
| [copyTo(View[] array, int arrayIndex)](#copyTo-com.aspose.tasks.View---int-) | Copia los elementos de esta colección al array especificado, comenzando en el índice del array especificado. |
| [getByName(String viewName)](#getByName-java.lang.String-) | Busca una View por el nombre y devuelve la primera aparición dentro de la colección. |
| [getByViewScreen(int screen)](#getByViewScreen-int-) | Busca una View con la propiedad Screen especificada y devuelve la primera aparición dentro de la colección. |
| [getParentProject()](#getParentProject--) | Obtiene el padre del objeto View. |
| [iterator()](#iterator--) | Devuelve un iterador sobre los elementos contenidos en esta colección. |
| [remove(View item)](#remove-com.aspose.tasks.View-) | Elimina la primera aparición de un objeto específico de esta colección. |
| [size()](#size--) | Obtiene el número de elementos contenidos en esta colección. |
| [toList()](#toList--) | Convierte una colección de vistas a una lista de objetos [View](../../com.aspose.tasks/view). |
### add(View item) {#add-com.aspose.tasks.View-}
```
public final boolean add(View item)
```


Agrega el elemento especificado a esta colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | el elemento especificado para agregar a esta colección. |

**Returns:**
boolean - true si la operación fue exitosa.
### clear() {#clear--}
```
public final void clear()
```


Elimina todos los elementos de esta colección.

### contains(View item) {#contains-com.aspose.tasks.View-}
```
public final boolean contains(View item)
```


Devuelve true si el elemento especificado se encuentra en esta colección; de lo contrario, false.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | el elemento especificado para buscar. |

**Returns:**
boolean - true si el elemento especificado se encuentra en esta colección; de lo contrario, false.
### copyTo(View[] array, int arrayIndex) {#copyTo-com.aspose.tasks.View---int-}
```
public final void copyTo(View[] array, int arrayIndex)
```


Copia los elementos de esta colección al array especificado, comenzando en el índice del array especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| array | [View\[\]](../../com.aspose.tasks/view) | el array unidimensional especificado al que copiar los elementos |
| arrayIndex | int | el índice basado en cero del array especificado en el que comienza la copia. |

### getByName(String viewName) {#getByName-java.lang.String-}
```
public final View getByName(String viewName)
```


Busca una View por el nombre y devuelve la primera aparición dentro de la colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| viewName | java.lang.String | Nombre de la View a buscar. |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection with the specified name, if found; otherwise, null.
### getByViewScreen(int screen) {#getByViewScreen-int-}
```
public final View getByViewScreen(int screen)
```


Busca una View con la propiedad Screen especificada y devuelve la primera aparición dentro de la colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| screen | int | Valor de enumeración [ViewScreen](../../com.aspose.tasks/viewscreen). |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection which Screen property matches the specified screen argument, if found; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Obtiene el padre del objeto View. Solo lectura [Project](../../com.aspose.tasks/project).

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the View object.
### iterator() {#iterator--}
```
public Iterator<View> iterator()
```


Devuelve un iterador sobre los elementos contenidos en esta colección.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.View&gt; - iterador de colección.
### remove(View item) {#remove-com.aspose.tasks.View-}
```
public final boolean remove(View item)
```


Elimina la primera aparición de un objeto específico de esta colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | el objeto especificado para eliminar. |

**Returns:**
boolean - true si el objeto especificado se eliminó correctamente de esta colección; de lo contrario, false.
### size() {#size--}
```
public final int size()
```


Obtiene el número de elementos contenidos en esta colección.

**Returns:**
int - el número de elementos contenidos en esta colección.
### toList() {#toList--}
```
public final List<View> toList()
```


Convierte una colección de vistas a una lista de objetos [View](../../com.aspose.tasks/view).

**Returns:**
java.util.List&lt;com.aspose.tasks.View&gt; - Lista genérica de objetos [View](../../com.aspose.tasks/view).
