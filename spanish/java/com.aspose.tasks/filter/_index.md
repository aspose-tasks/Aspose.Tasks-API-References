---
title: "Filtro"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa un filtro en Project."
type: docs
weight: 91
url: /es/java/com.aspose.tasks/filter/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable, com.aspose.ms.System.IEquatable
```
public final class Filter implements Comparable<Filter>, System.IEquatable<Filter>
```

Representa un filtro en Project.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [Filter()](#Filter--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [compareTo(Filter other)](#compareTo-com.aspose.tasks.Filter-) | Compara esta instancia con la instancia especificada de la clase [Filter](../../com.aspose.tasks/filter) y devuelve una indicación de su orden relativo. |
| [equals(Filter other)](#equals-com.aspose.tasks.Filter-) | Devuelve un valor que indica si esta instancia es igual al objeto AssignmentBaseline especificado. |
| [equals(Object obj)](#equals-java.lang.Object-) | Devuelve un valor que indica si esta instancia es igual al objeto AssignmentBaseline especificado. |
| [getCriteria()](#getCriteria--) | Obtiene los criterios que las tareas o recursos deben cumplir para mostrarse en la vista MSP. |
| [getFilterType()](#getFilterType--) | Obtiene el tipo del filtro. |
| [getIndex()](#getIndex--) | Obtiene el índice de un objeto [Filter](../../com.aspose.tasks/filter) en el objeto que contiene los Filters. |
| [getName()](#getName--) | Obtiene el nombre de un objeto Filter. |
| [getShowInMenu()](#getShowInMenu--) | Obtiene un valor que indica si el proyecto muestra el nombre del filtro en la lista desplegable Filter en la pestaña View de la Ribbon. |
| [getShowRelatedSummaryRows()](#getShowRelatedSummaryRows--) | Obtiene un valor que indica si se muestran filas de resumen relacionadas para el filtro. |
| [getUid()](#getUid--) | Obtiene el identificador único de un filtro. |
| [hashCode()](#hashCode--) | Devuelve un valor de código hash para el filtro. |
| [op_Equality(Filter a, Filter b)](#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| [op_GreaterThan(Filter a, Filter b)](#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Devuelve un valor que indica si esta instancia es mayor que un objeto especificado. |
| [op_GreaterThanOrEqual(Filter a, Filter b)](#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Devuelve un valor que indica si esta instancia es mayor o igual que un objeto especificado. |
| [op_Inequality(Filter a, Filter b)](#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Devuelve un valor que indica si esta instancia no es igual a un objeto especificado. |
| [op_LessThan(Filter a, Filter b)](#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Devuelve un valor que indica si esta instancia es menor que un objeto especificado. |
| [op_LessThanOrEqual(Filter a, Filter b)](#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Devuelve un valor que indica si esta instancia es menor o igual que un objeto especificado. |
| [setCriteria(FilterCriteria value)](#setCriteria-com.aspose.tasks.FilterCriteria-) | Establece los criterios que las tareas o recursos deben cumplir para mostrarse en la vista MSP. |
| [setFilterType(int value)](#setFilterType-int-) | El tipo del filtro. |
| [setName(String value)](#setName-java.lang.String-) | Establece el nombre de un objeto Filter. |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | Establece un valor que indica si el proyecto muestra el nombre del filtro en la lista desplegable Filter en la pestaña View de la Ribbon. |
| [setShowRelatedSummaryRows(boolean value)](#setShowRelatedSummaryRows-boolean-) | Establece un valor que indica si se muestran filas de resumen relacionadas para el filtro. |
### Filter() {#Filter--}
```
public Filter()
```


### compareTo(Filter other) {#compareTo-com.aspose.tasks.Filter-}
```
public final int compareTo(Filter other)
```


Compara esta instancia con la instancia especificada de la clase [Filter](../../com.aspose.tasks/filter) y devuelve una indicación de su orden relativo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | la instancia especificada de la clase [Filter](../../com.aspose.tasks/filter) para comparar con este objeto. |

**Returns:**
int - una indicación de su orden relativo.
### equals(Filter other) {#equals-com.aspose.tasks.Filter-}
```
public final boolean equals(Filter other)
```


Devuelve un valor que indica si esta instancia es igual al objeto AssignmentBaseline especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | el objeto AssignmentBaseline especificado para comparar con esta instancia. |

**Returns:**
boolean - devuelve true si esta instancia es igual al objeto AssignmentBaseline especificado; de lo contrario, false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Devuelve un valor que indica si esta instancia es igual al objeto AssignmentBaseline especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | java.lang.Object | el objeto AssignmentBaseline especificado para comparar con esta instancia. |

**Returns:**
boolean - devuelve true si esta instancia es igual al objeto AssignmentBaseline especificado; de lo contrario, false.
### getCriteria() {#getCriteria--}
```
public final FilterCriteria getCriteria()
```


Obtiene los criterios que las tareas o recursos deben cumplir para mostrarse en la vista MSP.

**Returns:**
[FilterCriteria](../../com.aspose.tasks/filtercriteria) - the criteria that tasks or resources must meet to be displayed in MSP view.
### getFilterType() {#getFilterType--}
```
public final int getFilterType()
```


Obtiene el tipo del filtro.

**Returns:**
int - el tipo del filtro.
### getIndex() {#getIndex--}
```
public final int getIndex()
```


Obtiene el índice de un objeto [Filter](../../com.aspose.tasks/filter) en el objeto que contiene los Filters.

**Returns:**
int - el índice de un objeto [Filter](../../com.aspose.tasks/filter) en el objeto que contiene los Filters.
### getName() {#getName--}
```
public final String getName()
```


Obtiene el nombre de un objeto Filter.

**Returns:**
java.lang.String - el nombre de un objeto Filter.
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


Obtiene un valor que indica si el proyecto muestra el nombre del filtro en la lista desplegable Filter en la pestaña View de la Ribbon.

**Returns:**
boolean - un valor que indica si el proyecto muestra el nombre del filtro en la lista desplegable Filtro en la pestaña Vista de la cinta.
### getShowRelatedSummaryRows() {#getShowRelatedSummaryRows--}
```
public final boolean getShowRelatedSummaryRows()
```


Obtiene un valor que indica si se muestran filas de resumen relacionadas para el filtro.

**Returns:**
boolean - un valor que indica si se muestran filas de resumen relacionadas para el filtro.
### getUid() {#getUid--}
```
public final int getUid()
```


Obtiene el identificador único de un filtro.

**Returns:**
int - el identificador único de un filtro.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Devuelve un valor de código hash para el filtro.

**Returns:**
int - devuelve un valor de código hash para este objeto.
### op_Equality(Filter a, Filter b) {#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Equality(Filter a, Filter b)
```


Devuelve un valor que indica si esta instancia es igual a un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | El primer filtro. |
| b | [Filter](../../com.aspose.tasks/filter) | El segundo filtro. |

**Returns:**
boolean - un valor que indica si esta instancia es igual a un objeto especificado
### op_GreaterThan(Filter a, Filter b) {#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThan(Filter a, Filter b)
```


Devuelve un valor que indica si esta instancia es mayor que un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | El primer filtro. |
| b | [Filter](../../com.aspose.tasks/filter) | El segundo filtro. |

**Returns:**
boolean - un valor que indica si esta instancia es mayor que un objeto especificado
### op_GreaterThanOrEqual(Filter a, Filter b) {#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThanOrEqual(Filter a, Filter b)
```


Devuelve un valor que indica si esta instancia es mayor o igual que un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | El primer filtro. |
| b | [Filter](../../com.aspose.tasks/filter) | El segundo filtro. |

**Returns:**
boolean - un valor que indica si esta instancia es mayor o igual que un objeto especificado
### op_Inequality(Filter a, Filter b) {#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Inequality(Filter a, Filter b)
```


Devuelve un valor que indica si esta instancia no es igual a un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | El primer filtro. |
| b | [Filter](../../com.aspose.tasks/filter) | El segundo filtro. |

**Returns:**
boolean - un valor que indica si esta instancia no es igual a un objeto especificado
### op_LessThan(Filter a, Filter b) {#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThan(Filter a, Filter b)
```


Devuelve un valor que indica si esta instancia es menor que un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | El primer filtro. |
| b | [Filter](../../com.aspose.tasks/filter) | El segundo filtro. |

**Returns:**
boolean - un valor que indica si esta instancia es menor que un objeto especificado
### op_LessThanOrEqual(Filter a, Filter b) {#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThanOrEqual(Filter a, Filter b)
```


Devuelve un valor que indica si esta instancia es menor o igual que un objeto especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | El primer filtro. |
| b | [Filter](../../com.aspose.tasks/filter) | El segundo filtro. |

**Returns:**
boolean - un valor que indica si esta instancia es menor o igual que un objeto especificado
### setCriteria(FilterCriteria value) {#setCriteria-com.aspose.tasks.FilterCriteria-}
```
public final void setCriteria(FilterCriteria value)
```


Establece los criterios que las tareas o recursos deben cumplir para mostrarse en la vista MSP.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [FilterCriteria](../../com.aspose.tasks/filtercriteria) | los criterios que las tareas o recursos deben cumplir para mostrarse en la vista MSP. |

### setFilterType(int value) {#setFilterType-int-}
```
public final void setFilterType(int value)
```


El tipo del filtro.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el tipo del filtro. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Establece el nombre de un objeto Filter.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | el nombre de un objeto Filter. |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


Establece un valor que indica si el proyecto muestra el nombre del filtro en la lista desplegable Filter en la pestaña View de la Ribbon.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si el proyecto muestra el nombre del filtro en la lista desplegable Filtro en la pestaña Vista de la cinta. |

### setShowRelatedSummaryRows(boolean value) {#setShowRelatedSummaryRows-boolean-}
```
public final void setShowRelatedSummaryRows(boolean value)
```


Establece un valor que indica si se muestran filas de resumen relacionadas para el filtro.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se muestran filas de resumen relacionadas para el filtro. |

