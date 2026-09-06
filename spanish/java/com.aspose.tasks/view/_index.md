---
title: "Vista"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa una vista en Project."
type: docs
weight: 342
url: /es/java/com.aspose.tasks/view/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable
```
public class View implements Comparable<View>
```

Representa una vista en Project.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [View()](#View--) | Inicializa una nueva instancia de la clase [View](../../com.aspose.tasks/view). |
## Métodos

| Método | Descripción |
| --- | --- |
| [compareTo(View other)](#compareTo-com.aspose.tasks.View-) | Compara la instancia actual con otro objeto del mismo tipo y devuelve un entero que indica si la instancia actual precede, sigue o se encuentra en la misma posición en el orden de clasificación que el otro objeto. |
| [equals(Object obj)](#equals-java.lang.Object-) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| [forViewScreen(int viewScreen)](#forViewScreen-int-) | Construye una nueva instancia de la clase [View](../../com.aspose.tasks/view). |
| [getFilter()](#getFilter--) | Obtiene un filtro usado en una vista única. |
| [getGroup()](#getGroup--) | Obtiene un grupo de la vista única. |
| [getHighlightFilter()](#getHighlightFilter--) | Obtiene un valor que indica si Microsoft Project resalta el filtro para una vista única. |
| [getName()](#getName--) | Obtiene el nombre de un objeto View. |
| [getPageInfo()](#getPageInfo--) | Obtiene una instancia de la clase `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)). |
| [getParentProject()](#getParentProject--) | Obtiene el padre del objeto View. |
| [getScreen()](#getScreen--) | Obtiene el tipo de pantalla para la vista única. |
| [getShowInMenu()](#getShowInMenu--) | Obtiene un valor que indica si Microsoft Project muestra el nombre de la vista única en la lista desplegable Vista o Otras Vistas en la cinta de opciones. |
| [getTable()](#getTable--) | Obtiene una tabla de la vista única. |
| [getType()](#getType--) | Obtiene el tipo de elemento en la vista única, como tareas o recursos. |
| [getUid()](#getUid--) | Obtiene el identificador único de una vista. |
| [getVisualObjectsPlacements()](#getVisualObjectsPlacements--) | Obtiene una colección de objetos que representan la ubicación y apariencia de [OleObject](../../com.aspose/tasks/oleobject) en la vista. |
| [hashCode()](#hashCode--) | Devuelve un valor de código hash para la instancia de la clase [Resource](../../com.aspose.tasks/resource). |
| [op_Equality(View a, View b)](#op-Equality-com.aspose.tasks.View-com.aspose.tasks.View-) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| [op_GreaterThan(View a, View b)](#op-GreaterThan-com.aspose.tasks.View-com.aspose.tasks.View-) | Devuelve un valor que indica si esta instancia es mayor que un objeto especificado. |
| [op_GreaterThanOrEqual(View a, View b)](#op-GreaterThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-) | Devuelve un valor que indica si esta instancia es mayor o igual que un objeto especificado. |
| [op_Inequality(View a, View b)](#op-Inequality-com.aspose.tasks.View-com.aspose.tasks.View-) | Devuelve un valor que indica si esta instancia no es igual a un objeto especificado. |
| [op_LessThan(View a, View b)](#op-LessThan-com.aspose.tasks.View-com.aspose.tasks.View-) | Devuelve un valor que indica si esta instancia es menor que un objeto especificado. |
| [op_LessThanOrEqual(View a, View b)](#op-LessThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-) | Devuelve un valor que indica si esta instancia es menor o igual que un objeto especificado. |
| [setFilter(Filter value)](#setFilter-com.aspose.tasks.Filter-) | Establece un filtro usado en una vista única. |
| [setGroup(Group value)](#setGroup-com.aspose.tasks.Group-) | Establece un grupo de la vista única. |
| [setHighlightFilter(boolean value)](#setHighlightFilter-boolean-) | Establece un valor que indica si Microsoft Project resalta el filtro para una vista única. |
| [setName(String value)](#setName-java.lang.String-) | Establece el nombre de un objeto View. |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | Establece un valor que indica si Microsoft Project muestra el nombre de la vista única en la lista desplegable Vista o Otras Vistas en la cinta de opciones. |
| [setTable(Table value)](#setTable-com.aspose.tasks.Table-) | Establece una tabla de la vista única. |
### View() {#View--}
```
public View()
```


Inicializa una nueva instancia de la clase [View](../../com.aspose.tasks/view).

### compareTo(View other) {#compareTo-com.aspose.tasks.View-}
```
public final int compareTo(View other)
```


Compara la instancia actual con otro objeto del mismo tipo y devuelve un entero que indica si la instancia actual precede, sigue o se encuentra en la misma posición en el orden de clasificación que el otro objeto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| other | [View](../../com.aspose.tasks/view) | el objeto View especificado para comparar esta instancia con. |

**Returns:**
int - Un entero con signo de 32 bits que indica el orden relativo de los objetos comparados. El valor de retorno tiene los siguientes significados: Valor Significado Menor que cero Esta instancia precede a `other` en el orden de clasificación. Cero Esta instancia se encuentra en la misma posición en el orden de clasificación que `other`. Mayor que cero Esta instancia sigue a `other` en el orden de clasificación.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Devuelve un valor que indica si esta instancia es igual a un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | java.lang.Object | El objeto para comparar con esta instancia. |

**Returns:**
boolean - **True** si el objeto especificado es una View que tiene el mismo valor Uid que esta instancia; de lo contrario, **false**.
### forViewScreen(int viewScreen) {#forViewScreen-int-}
```
public static View forViewScreen(int viewScreen)
```


Construye una nueva instancia de la clase [View](../../com.aspose.tasks/view).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| viewScreen | int | El tipo de pantalla para la cual la vista puede mostrarse. |

**Returns:**
[View](../../com.aspose.tasks/view) - Constructed view.
### getFilter() {#getFilter--}
```
public final Filter getFilter()
```


Obtiene un filtro usado en una vista única.

**Returns:**
[Filter](../../com.aspose.tasks/filter) - a filter used in a single view.
### getGroup() {#getGroup--}
```
public final Group getGroup()
```


Obtiene un grupo de la vista única.

**Returns:**
[Group](../../com.aspose.tasks/group) - a group of the single view.
### getHighlightFilter() {#getHighlightFilter--}
```
public final boolean getHighlightFilter()
```


Obtiene un valor que indica si Microsoft Project resalta el filtro para una vista única.

**Returns:**
boolean - un valor que indica si Microsoft Project resalta el filtro para una vista única.
### getName() {#getName--}
```
public final String getName()
```


Obtiene el nombre de un objeto View.

**Returns:**
java.lang.String - el nombre de un objeto View.
### getPageInfo() {#getPageInfo--}
```
public final PageInfo getPageInfo()
```


Obtiene una instancia de la clase `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)). Representa los datos de configuración de página que están presentes en el formato de archivo mpp.

**Returns:**
[PageInfo](../../com.aspose.tasks/pageinfo) - an instance of the `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)) class.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Obtiene el padre del objeto View. Solo lectura [Project](../../com.aspose.tasks/project).

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the View object.
### getScreen() {#getScreen--}
```
public final int getScreen()
```


Obtiene el tipo de pantalla para la vista única. Solo lectura [ViewScreen](../../com.aspose.tasks/viewscreen).

**Returns:**
int - el tipo de pantalla para la vista única.
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


Obtiene un valor que indica si Microsoft Project muestra el nombre de la vista única en la lista desplegable Vista o Otras Vistas en la cinta de opciones.

**Returns:**
boolean - un valor que indica si Microsoft Project muestra el nombre de la vista única en la lista desplegable Vista o Otras Vistas en la cinta de opciones.
### getTable() {#getTable--}
```
public final Table getTable()
```


Obtiene una tabla de la vista única.

**Returns:**
[Table](../../com.aspose.tasks/table) - a table of the single view.
### getType() {#getType--}
```
public final int getType()
```


Obtiene el tipo de elemento en la vista única, como tareas o recursos. Solo lectura [ItemType](../../com.aspose.tasks/itemtype).

**Returns:**
int - el tipo de elemento en la vista única, como tareas o recursos.
### getUid() {#getUid--}
```
public final int getUid()
```


Obtiene el identificador único de una vista.

**Returns:**
int - el identificador único de una vista.
### getVisualObjectsPlacements() {#getVisualObjectsPlacements--}
```
public final List<VisualObjectPlacement> getVisualObjectsPlacements()
```


Obtiene una colección de objetos que representan la ubicación y apariencia de [OleObject](../../com.aspose/tasks/oleobject) en la vista.

**Returns:**
java.util.List&lt;com.aspose.tasks.VisualObjectPlacement&gt; - una colección de objetos que representan la ubicación y apariencia de [OleObject](../../com.aspose.tasks/oleobject) en la vista.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Devuelve un valor de código hash para la instancia de la clase [Resource](../../com.aspose.tasks/resource).

**Returns:**
int - devuelve un valor de código hash para este objeto.
### op_Equality(View a, View b) {#op-Equality-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_Equality(View a, View b)
```


Devuelve un valor que indica si esta instancia es igual a un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | La primera vista. |
| b | [View](../../com.aspose.tasks/view) | La segunda vista. |

**Returns:**
boolean - un valor que indica si esta instancia es igual a un objeto especificado
### op_GreaterThan(View a, View b) {#op-GreaterThan-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_GreaterThan(View a, View b)
```


Devuelve un valor que indica si esta instancia es mayor que un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | La primera vista. |
| b | [View](../../com.aspose.tasks/view) | La segunda vista. |

**Returns:**
boolean - un valor que indica si esta instancia es mayor que un objeto especificado
### op_GreaterThanOrEqual(View a, View b) {#op-GreaterThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_GreaterThanOrEqual(View a, View b)
```


Devuelve un valor que indica si esta instancia es mayor o igual que un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | La primera vista. |
| b | [View](../../com.aspose.tasks/view) | La segunda vista. |

**Returns:**
boolean - un valor que indica si esta instancia es mayor o igual que un objeto especificado
### op_Inequality(View a, View b) {#op-Inequality-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_Inequality(View a, View b)
```


Devuelve un valor que indica si esta instancia no es igual a un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | La primera vista. |
| b | [View](../../com.aspose.tasks/view) | La segunda vista. |

**Returns:**
boolean - un valor que indica si esta instancia no es igual a un objeto especificado
### op_LessThan(View a, View b) {#op-LessThan-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_LessThan(View a, View b)
```


Devuelve un valor que indica si esta instancia es menor que un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | El primer filtro. |
| b | [View](../../com.aspose.tasks/view) | El segundo filtro. |

**Returns:**
boolean - un valor que indica si esta instancia es menor que un objeto especificado
### op_LessThanOrEqual(View a, View b) {#op-LessThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_LessThanOrEqual(View a, View b)
```


Devuelve un valor que indica si esta instancia es menor o igual que un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | La primera vista. |
| b | [View](../../com.aspose.tasks/view) | La segunda vista. |

**Returns:**
boolean - un valor que indica si esta instancia es menor o igual que un objeto especificado
### setFilter(Filter value) {#setFilter-com.aspose.tasks.Filter-}
```
public final void setFilter(Filter value)
```


Establece un filtro usado en una vista única.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Filter](../../com.aspose.tasks/filter) | un filtro usado en una vista única. |

### setGroup(Group value) {#setGroup-com.aspose.tasks.Group-}
```
public final void setGroup(Group value)
```


Establece un grupo de la vista única.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Group](../../com.aspose.tasks/group) | un grupo de la vista única. |

### setHighlightFilter(boolean value) {#setHighlightFilter-boolean-}
```
public final void setHighlightFilter(boolean value)
```


Establece un valor que indica si Microsoft Project resalta el filtro para una vista única.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si Microsoft Project resalta el filtro para una vista única. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Establece el nombre de un objeto View.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | el nombre de un objeto Vista. |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


Establece un valor que indica si Microsoft Project muestra el nombre de la vista única en la lista desplegable Vista o Otras Vistas en la cinta de opciones.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si Microsoft Project muestra el nombre de la vista única en la lista desplegable Vista o Otras Vistas en la cinta. |

### setTable(Table value) {#setTable-com.aspose.tasks.Table-}
```
public final void setTable(Table value)
```


Establece una tabla de la vista única.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [Table](../../com.aspose.tasks/table) | una tabla de la vista única. |

