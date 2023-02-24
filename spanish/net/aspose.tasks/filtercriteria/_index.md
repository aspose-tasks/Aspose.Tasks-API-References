---
title: Class FilterCriteria
second_title: Referencia de Aspose.Tasks para la API de .NET
description: Aspose.Tasks.FilterCriteria clase. Define los criterios que deben cumplir las tareas o los recursos para que se muestren en la vista MSP.
type: docs
weight: 630
url: /es/net/aspose.tasks/filtercriteria/
---
## FilterCriteria class

Define los criterios que deben cumplir las tareas o los recursos para que se muestren en la vista MSP.

```csharp
public class FilterCriteria
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [FilterCriteria](filtercriteria/)() | Constructor predeterminado |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CriteriaRows](../../aspose.tasks/filtercriteria/criteriarows/) { get; } | Obtiene la lista de niños`FilterCriteria` filas. Si el filtro contiene más de una fila de criterios, el efecto de un operador Y es que se deben cumplir los criterios de ambas filas para que se muestre la tarea o el recurso como resultado de este filtro. El efecto de un operador O operador es que se deben cumplir los criterios para una u otra fila. |
| [Field](../../aspose.tasks/filtercriteria/field/) { get; set; } | Obtiene o establece un[`Field`](./field/) para cambiar. |
| [Operation](../../aspose.tasks/filtercriteria/operation/) { get; set; } | Obtiene o establece el criterio establecido con FieldName, Test y Value se relaciona con otros criterios en el filtro. |
| [Test](../../aspose.tasks/filtercriteria/test/) { get; set; } | Obtiene o establece el tipo de comparación realizada entre FieldName y Value que actúa como criterio de selección del filtro. [`FilterComparisonType`](../filtercomparisontype/) |
| [Values](../../aspose.tasks/filtercriteria/values/) { get; } | Obtiene los valores del objeto para compararlos con el valor del campo especificado con FieldName. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [ToString](../../aspose.tasks/filtercriteria/tostring/)() | Devuelve la representación de cadena de la instancia del`FilterCriteria` clase. |

### Ver también

* espacio de nombres [Aspose.Tasks](../../aspose.tasks/)
* asamblea [Aspose.Tasks](../../)


