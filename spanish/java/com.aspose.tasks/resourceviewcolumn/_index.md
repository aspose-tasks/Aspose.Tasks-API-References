---
title: "ResourceViewColumn"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Clase de vista de proyectos utilizada en la vista ResourceUsage y en la vista ResourceSheet."
type: docs
weight: 261
url: /es/java/com.aspose.tasks/resourceviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class ResourceViewColumn extends ViewColumn
```

Clase de vista del proyecto utilizada en la vista ResourceUsage y la vista ResourceSheet.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-) | Inicializa una nueva instancia de la clase [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn). |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-) | Inicializa una nueva instancia de la clase [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn). |
| [ResourceViewColumn(int width, int field)](#ResourceViewColumn-int-int-) | Inicializa una nueva instancia de la clase [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getColumnText(Resource resource)](#getColumnText-com.aspose.tasks.Resource-) | Convierte el recurso actual al texto de la columna. |
| [getField()](#getField--) | Devuelve el campo de la columna. |
| [setField(int value)](#setField-int-) | Establece el campo de la columna. |
### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)
```


Inicializa una nueva instancia de la clase [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | Nombre de la columna. |
| width | int | Ancho de la columna en píxeles. |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | Convertidor de datos de recurso a texto de columna. |
| campo | int | Campo de columna. |

### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)
```


Inicializa una nueva instancia de la clase [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | Nombre de la columna. |
| width | int | Ancho de la columna en píxeles. |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | Convertidor de datos de recurso a texto de columna. |

### ResourceViewColumn(int width, int field) {#ResourceViewColumn-int-int-}
```
public ResourceViewColumn(int width, int field)
```


Inicializa una nueva instancia de la clase [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| width | int | Ancho de columna en píxeles. |
| campo | int | Campo de columna. |

### getColumnText(Resource resource) {#getColumnText-com.aspose.tasks.Resource-}
```
public final String getColumnText(Resource resource)
```


Convierte el recurso actual al texto de la columna.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| resource | [Resource](../../com.aspose.tasks/resource) | Recurso actual. |

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

