---
title: "FilterCriteria"
second_title: "Referencia de API de Aspose.Tasks para Python vía .NET"
description: 
type: docs
weight: 350
url: /es/python-net/aspose.tasks/filtercriteria/
---

## FilterCriteria class

Define los criterios que las tareas o recursos deben cumplir para mostrarse en la vista MSP.

El tipo FilterCriteria expone los siguientes miembros:
## Constructores
| Nombre | Descripción |
| :- | :- |
| FilterCriteria() | Inicializa una nueva instancia de la clase FilterCriteria |
## Propiedades
| Nombre | Descripción |
| :- | :- |
| operación | Obtiene o establece el criterio establecido con FieldName, Test y Value que se relaciona con otros criterios en el filtro. |
| field | Obtiene o establece un [field](/tasks/python-net/aspose.tasks/filtercriteria/) para cambiar. |
| test | Obtiene o establece el tipo de comparación realizado entre FieldName y Value que actúa como criterio de selección para el filtro.<br/>            [FilterComparisonType](/tasks/python-net/aspose.tasks/filtercomparisontype/) |
| values | Obtiene los valores de objeto para comparar con el valor del campo especificado con FieldName. |
| criteria_rows | Obtiene la lista de filas hijas de [FilterCriteria](/tasks/python-net/aspose.tasks/filtercriteria/).<br/>            Si el filtro contiene más de una fila de criterio, entonces el efecto de un operador And es que los criterios de ambas filas deben cumplirse para que la tarea o recurso se muestre como resultado de este filtro.<br/>            El efecto de un operador Or es que los criterios de una u otra fila deben cumplirse. |
## Métodos
| Nombre | Descripción |
| :- | :- |
| is_field_value() | Obtiene si el valor del lado derecho de FilterCriteria es una referencia a un campo, no un valor constante. |
| set_value_field(value) | Establece el campo cuyo valor será comparado con el valor del campo especificado por FieldName. |

### Ver también

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

