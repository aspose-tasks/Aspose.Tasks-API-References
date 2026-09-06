---
title: "AssignmentViewColumn"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Clase de vista de proyectos."
type: docs
weight: 19
url: /es/java/com.aspose.tasks/assignmentviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public class AssignmentViewColumn extends ViewColumn
```

Clase de vista del proyecto.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)](#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-) | Inicializa una nueva instancia de la clase AssignmentViewColumn. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getColumnText(ResourceAssignment assignment)](#getColumnText-com.aspose.tasks.ResourceAssignment-) | Convierte la asignación de recurso actual al texto de la columna. |
| [getField()](#getField--) | Devuelve el campo de la columna. |
| [setField(int value)](#setField-int-) | Establece el campo de la columna. |
### AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter) {#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-}
```
public AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)
```


Inicializa una nueva instancia de la clase AssignmentViewColumn.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | Nombre de la columna. |
| width | int | Ancho de la columna en píxeles. |
| converter | [AssignmentToColumnTextConverter](../../com.aspose.tasks/assignmenttocolumntextconverter) | Convertidor de datos de asignación a texto de columna. |

### getColumnText(ResourceAssignment assignment) {#getColumnText-com.aspose.tasks.ResourceAssignment-}
```
public String getColumnText(ResourceAssignment assignment)
```


Convierte la asignación de recurso actual al texto de la columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| assignment | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | Asignación actual. |

**Returns:**
java.lang.String - El texto de la columna.
### getField() {#getField--}
```
public int getField()
```


Devuelve el campo de la columna. `Field`.

**Returns:**
int - valor del campo de la columna.
### setField(int value) {#setField-int-}
```
public void setField(int value)
```


Establece el campo de la columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | valor del campo de la columna. |

