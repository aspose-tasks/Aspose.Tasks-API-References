---
title: "ExtendedAttributeDefinition"
second_title: "Referencia de API de Aspose.Tasks para Python vía .NET"
description: 
type: docs
weight: 310
url: /es/python-net/aspose.tasks/extendedattributedefinition/
---

## ExtendedAttributeDefinition class

Representa una definición de atributo extendido asociada a un proyecto.

El tipo ExtendedAttributeDefinition expone los siguientes miembros:
## Propiedades
| Nombre | Descripción |
| :- | :- |
| field_id | Obtiene o establece el identificador del proyecto de un campo personalizado.<br/>            Utilice la representación en cadena de una constante de la clase [ExtendedAttributeTask](/tasks/python-net/aspose.tasks/extendedattributetask/) para especificar la propiedad [field_id](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |
| field_name | Obtiene el nombre de un campo personalizado. |
| cf_type | Obtiene el tipo de un campo personalizado. |
| guid | Obtiene o establece el Guid de un campo personalizado. |
| element_type | Obtiene o establece el atributo extendido asociado<br/>            con una tarea, un recurso o una asignación. |
| max_multi_values | Obtiene o establece el número máximo de valores que puede establecer en una lista de selección. |
| user_def | Obtiene o establece un valor que indica si un campo personalizado está definido por el usuario. |
| alias | Obtiene o establece el alias de un campo personalizado. |
| secondary_pid | Obtiene o establece el PID secundario de un campo personalizado. |
| auto_roll_down | Obtiene o establece un valor que indica si se ha habilitado un descenso automático a asignaciones. |
| default_guid | Obtiene o establece el GUID de la entrada predeterminada de la tabla de búsqueda. |
| lookup_uid | Obtiene un GUID de la tabla de búsqueda asociada a un campo personalizado. |
| phonetics_alias | Obtiene o establece la pronunciación fonética del alias de un campo personalizado. |
| rollup_type | Obtiene o establece la forma en que se calculan los acumulados. |
| calculation_type | Obtiene o establece el tipo de cálculo del valor del atributo personalizado. |
| summary_rows_calculation_type | Obtiene o establece el tipo de cálculo del valor del atributo personalizado para filas de resumen. |
| formula | Obtiene o establece la fórmula que Microsoft Project utiliza para rellenar un campo de tarea personalizado. |
| graphical_indicator | Obtiene o establece la información de indicadores gráficos asociada con el atributo extendido.<br/>            Aplicable al formato MPP. |
| restrict_values | Obtiene o establece un valor que indica si los valores de los campos personalizados están restringidos a los valores en la [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |
| valuelist_sort_order | Obtiene o establece la forma en que se ordenan las listas de valores. Los valores son: 0=Descendente, 1=Ascendente. |
| append_new_values | Obtiene o establece un valor que indica si los nuevos valores añadidos a un proyecto se agregan automáticamente a la lista. |
| default | Obtiene o establece el valor predeterminado en la lista. |
| value_list | Obtiene la List<Value> ValueList. |
| secondary_guid | Obtiene o establece el GUID secundario del atributo extendido. |
| parent_project | Obtiene el proyecto principal para la instancia de [ExtendedAttributeDefinition](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |
## Métodos
| Nombre | Descripción |
| :- | :- |
| create_extended_attribute() | Crea un nuevo atributo extendido con el ID de campo que es igual al valor del ID de campo de este objeto. |
| create_extended_attribute(text_value) | Crea un nuevo atributo extendido con el ID de campo que es igual al valor del ID de campo de este objeto y el valor de texto especificado. |
| create_extended_attribute(numeric_value) | Crea un nuevo atributo extendido con el ID de campo que es igual al valor del ID de campo de este objeto y el valor numérico especificado. |
| create_extended_attribute(date_time_value) | Crea un nuevo atributo extendido con el ID de campo que es igual al valor del ID de campo de este objeto y el valor de fecha especificado. |
| create_extended_attribute(duration_value) | Crea un nuevo atributo extendido con el ID de campo que es igual al valor del ID de campo de este objeto y el valor de duración especificado. |
| create_extended_attribute(flag_value) | Crea un nuevo atributo extendido con el ID de campo que es igual al valor del ID de campo de este objeto y el valor de bandera especificado. |
| create_extended_attribute(lookup_value) | Crea un nuevo atributo extendido vinculado con el elemento [Value](/tasks/python-net/aspose.tasks/value/) especificado. |
| create_task_definition(custom_field_type, field_id, alias) | Método de fábrica que crea una definición de atributo extendido simple, que Microsoft Project muestra como "None".<br/>            Tiene [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) igual a [NONE](/tasks/python-net/aspose.tasks/calculationtype/) y solo se puede usar en Tareas.<br/>            Se requiere especificar |
| create_task_definition(field_id, alias) | Método de fábrica que crea una definición de atributo extendido simple, que Microsoft Project muestra como "None".<br/>            Tiene [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) igual a [NONE](/tasks/python-net/aspose.tasks/calculationtype/) y solo se puede usar en Tareas.<br/>            Se requiere especificar |
| create_resource_definition(custom_field_type, field_id, alias) | Método de fábrica que crea una definición de atributo extendido simple, que Microsoft Project muestra como "None".<br/>            Tiene [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) igual a [NONE](/tasks/python-net/aspose.tasks/calculationtype/) y solo se puede usar en Recursos.<br/>            Se requiere especificar |
| create_resource_definition(field_id, alias) | Método de fábrica que crea una definición de atributo extendido simple, que Microsoft Project muestra como "None".<br/>            Tiene [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) igual a [NONE](/tasks/python-net/aspose.tasks/calculationtype/) y solo se puede usar en Recursos.<br/>            Se requiere especificar |
| create_lookup_task_definition(field_id, alias) | Método de fábrica que crea una definición de atributo extendido con búsqueda.<br/>            Tiene [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) igual a [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) y solo se puede usar en Tareas.<br/>            Se requiere especificar |
| create_lookup_task_definition(custom_field_type, field_id, alias) | Método de fábrica que crea una definición de atributo extendido con búsqueda.<br/>            Tiene [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) igual a [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) y solo se puede usar en Tareas.<br/>            Se requiere especificar |
| create_lookup_resource_definition(field_id, alias) | Método de fábrica que crea una definición de atributo extendido con búsqueda.<br/>            Tiene [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) igual a [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) y solo se puede usar en Recursos.<br/>            Se requiere especificar |
| create_lookup_resource_definition(custom_field_type, field_id, alias) | Método de fábrica que crea una definición de atributo extendido con búsqueda.<br/>            Tiene [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) igual a [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) y solo se puede usar en Recursos.<br/>            Se requiere especificar |
| add_lookup_value(value) | Agrega un valor a la lista interna de búsqueda. Esta es la forma preferida de manipular la [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |
| remove_lookup_value(value) | Elimina un valor de la lista interna de búsqueda. Esta es la forma preferida de manipular la [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |

### Ver también

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

