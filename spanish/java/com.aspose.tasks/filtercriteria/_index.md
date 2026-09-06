---
title: "FilterCriteria"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Define los criterios que las tareas o recursos deben cumplir para mostrarse en la vista MSP."
type: docs
weight: 94
url: /es/java/com.aspose.tasks/filtercriteria/
---

**Inheritance:**
java.lang.Object
```
public class FilterCriteria
```

Define los criterios que las tareas o recursos deben cumplir para mostrarse en la vista MSP.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [FilterCriteria()](#FilterCriteria--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [getCriteriaRows()](#getCriteriaRows--) | Obtiene la lista de filas hijas de [FilterCriteria](../../com.aspose.tasks/filtercriteria). |
| [getField()](#getField--) | Obtiene un `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) para cambiar. |
| [getOperation()](#getOperation--) | Obtiene el criterio establecido con FieldName, Test y Value que se relaciona con otros criterios en el filtro. |
| [getTest()](#getTest--) | Obtiene el tipo de comparación realizado entre FieldName y Value que actúa como criterio de selección para el filtro. |
| [getValues()](#getValues--) | Obtiene los valores de objeto para comparar con el valor del campo especificado con FieldName. |
| [isValueAField()](#isValueAField--) | Obtiene si el valor del lado derecho de FilterCriteria es una referencia de campo, no un valor constante. |
| [isValueAField(int index)](#isValueAField-int-) | Obtiene si el valor en el índice de FilterCriteria es una referencia de campo, no un valor constante. |
| [setField(int value)](#setField-int-) | Establece un `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) para cambiar. |
| [setOperation(int value)](#setOperation-int-) | Establece el criterio establecido con FieldName, Test y Value que se relaciona con otros criterios en el filtro. |
| [setTest(int value)](#setTest-int-) | Establece el tipo de comparación realizado entre FieldName y Value que actúa como criterio de selección para el filtro. |
| [setValue(int index, Object value)](#setValue-int-java.lang.Object-) | Establece el valor de objeto en el índice para comparar con el valor del campo especificado por FieldName. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Establece el valor de objeto para comparar con el valor del campo especificado por FieldName. |
| [setValueByField(int value)](#setValueByField-int-) | Establece el campo cuyo valor será comparado con el valor del campo especificado por FieldName. |
| [setValueByField(int index, int value)](#setValueByField-int-int-) | Establece el campo en el índice cuyo valor será comparado con el valor del campo especificado por FieldName. |
| [toString()](#toString--) | Devuelve la representación en cadena de la instancia de la clase [FilterCriteria](../../com.aspose.tasks/filtercriteria). |
### FilterCriteria() {#FilterCriteria--}
```
public FilterCriteria()
```


### getCriteriaRows() {#getCriteriaRows--}
```
public final List<FilterCriteria> getCriteriaRows()
```


Obtiene la lista de filas hijas de [FilterCriteria](../../com.aspose.tasks/filtercriteria). Si el filtro contiene más de una fila de criterio, entonces el efecto del operador And es que los criterios de ambas filas deben cumplirse para que la tarea o recurso se muestre como resultado de este filtro. El efecto del operador Or es que se cumpla el criterio de una u otra fila.

**Returns:**
java.util.List&lt;com.aspose.tasks.FilterCriteria&gt; - la lista de filas hijas de [FilterCriteria](../../com.aspose.tasks/filtercriteria).
### getField() {#getField--}
```
public final int getField()
```


Obtiene un `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) para cambiar.

**Returns:**
int - un `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) para cambiar.
### getOperation() {#getOperation--}
```
public final int getOperation()
```


Obtiene el criterio establecido con FieldName, Test y Value que se relaciona con otros criterios en el filtro.

**Returns:**
int - el criterio establecido con FieldName, Test y Value que se relaciona con otros criterios en el filtro.
### getTest() {#getTest--}
```
public final int getTest()
```


Obtiene el tipo de comparación realizado entre FieldName y Value que actúa como criterio de selección para el filtro. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Returns:**
int - el tipo de comparación realizado entre FieldName y Value que actúa como criterio de selección para el filtro.
### getValues() {#getValues--}
```
public final Object[] getValues()
```


Obtiene los valores de objeto para comparar con el valor del campo especificado con FieldName.

**Returns:**
java.lang.Object[] - los valores de objeto para comparar con el valor del campo especificado con FieldName.
### isValueAField() {#isValueAField--}
```
public final boolean isValueAField()
```


Obtiene si el valor del lado derecho de FilterCriteria es una referencia de campo, no un valor constante.

**Returns:**
boolean - si el valor del lado derecho de FilterCriteria es una referencia de campo, no un valor constante.
### isValueAField(int index) {#isValueAField-int-}
```
public final boolean isValueAField(int index)
```


Obtiene si el valor en el índice de FilterCriteria es una referencia de campo, no un valor constante.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | el índice del valor |

**Returns:**
booleano - si el valor del lado derecho en el índice de FilterCriteria es una referencia a un campo, no un valor constante.
### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


Establece un `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) para cambiar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | int | un `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) para cambiar. |

### setOperation(int value) {#setOperation-int-}
```
public final void setOperation(int value)
```


Establece el criterio establecido con FieldName, Test y Value que se relaciona con otros criterios en el filtro.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el criterio establecido con FieldName, Test y Value se relaciona con otros criterios en el filtro. |

### setTest(int value) {#setTest-int-}
```
public final void setTest(int value)
```


Establece el tipo de comparación realizado entre FieldName y Value que actúa como criterio de selección para el filtro. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el tipo de comparación realizado entre FieldName y Value que actúa como criterio de selección para el filtro. |

### setValue(int index, Object value) {#setValue-int-java.lang.Object-}
```
public final void setValue(int index, Object value)
```


Establece el valor de objeto en el índice para comparar con el valor del campo especificado por FieldName.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | el índice del valor. |
| valor | java.lang.Object | valor de objeto que servirá como valor del lado derecho en el índice del criterio de filtro. |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public final void setValue(Object value)
```


Establece el valor de objeto para comparar con el valor del campo especificado por FieldName.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Object | valor de objeto que servirá como valor del lado derecho del criterio de filtro. |

### setValueByField(int value) {#setValueByField-int-}
```
public final void setValueByField(int value)
```


Establece el campo cuyo valor será comparado con el valor del campo especificado por FieldName.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | Campo que servirá como valor del lado derecho del criterio de filtro. |

### setValueByField(int index, int value) {#setValueByField-int-int-}
```
public final void setValueByField(int index, int value)
```


Establece el campo en el índice cuyo valor será comparado con el valor del campo especificado por FieldName.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | el índice del valor |
| valor | int | Campo que servirá como valor del lado derecho en el índice del criterio de filtro. |

### toString() {#toString--}
```
public String toString()
```


Devuelve la representación en cadena de la instancia de la clase [FilterCriteria](../../com.aspose.tasks/filtercriteria).

**Returns:**
java.lang.String - representación en cadena de este objeto.
