---
title: "Clase Aspose::Tasks::ExtendedAttributeDefinition"
linktitle: "ExtendedAttributeDefinition"
articleTitle: "ExtendedAttributeDefinition"
second_title: "Aspose.Tasks for C++"
description: "Representa una definición de atributo extendido asociada a un proyecto."
type: docs
weight: 10
url: /es/cpp/aspose.tasks/extendedattributedefinition/
---

## ExtendedAttributeDefinition class

Representa una definición de atributo extendido asociada a un proyecto.

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddLookupValue](./addlookupvalue/) | Agrega un valor a la lista de búsqueda interna. Esta es una forma preferible para manipulaciones con la ValueList. |
| [CreateExtendedAttribute (7 overloads)](./createextendedattribute/) | Crea un nuevo atributo extendido con el ID de campo que es igual al valor del ID de campo de este objeto. |
| [CreateLookupResourceDefinition (2 overloads)](./createlookupresourcedefinition/) | Método de fábrica que crea una definición de atributo extendido con búsqueda. Tiene CalculationType igual a Tasks::CalculationType::Lookup y solo puede usarse en Resources. Se requiere especificar customFieldType, fieldId y alias al llamar a este método. |
| [CreateLookupTaskDefinition (2 overloads)](./createlookuptaskdefinition/) | Método de fábrica que crea una definición de atributo extendido con búsqueda. Tiene CalculationType igual a Tasks::CalculationType::Lookup y solo puede usarse en Tasks. Se requiere especificar customFieldType, fieldId y alias al llamar a este método. |
| [CreateResourceDefinition (2 overloads)](./createresourcedefinition/) | Método de fábrica que crea una definición de atributo extendido simple, que Microsoft Project muestra como "None". Tiene CalculationType igual a Tasks::CalculationType::None y solo puede usarse en Resource. Se requiere especificar customFieldType, fieldId y alias al llamar a este método. |
| [CreateTaskDefinition (2 overloads)](./createtaskdefinition/) | Método de fábrica que crea una definición de atributo extendido simple, que Microsoft Project muestra como "None". Tiene CalculationType igual a Tasks::CalculationType::None y solo puede usarse en Tasks. Se requiere especificar customFieldType, fieldId y alias al llamar a este método. |
| [Equals](./equals/) | Devuelve una bandera que indica si esta instancia es igual al objeto especificado. |
| [get_Alias](./get_alias/) | Obtiene el alias de un campo personalizado. |
| [get_AppendNewValues](./get_appendnewvalues/) | Obtiene un valor que indica si los nuevos valores añadidos a un proyecto se añaden automáticamente a la lista. |
| [get_AutoRollDown](./get_autorolldown/) | Obtiene un valor que indica si se habilita una propagación automática a las asignaciones. |
| [get_CalculationType](./get_calculationtype/) | Obtiene el tipo de cálculo del valor del atributo personalizado. |
| [get_CfType](./get_cftype/) | Obtiene el tipo de un campo personalizado. |
| [get_Default](./get_default/) | Obtiene el valor predeterminado en la lista. |
| [get_DefaultGuid](./get_defaultguid/) | Obtiene el GUID de la entrada predeterminada de la tabla de búsqueda. |
| [get_ElementType](./get_elementtype/) | Obtiene si el atributo extendido está asociado a una tarea, un recurso o una asignación. |
| [get_FieldId](./get_fieldid/) | Obtiene lo que corresponde al id del proyecto de un campo personalizado. Utilice la representación de cadena de una constante de la clase Aspose::Tasks::ExtendedAttributeTask para especificar la propiedad FieldId. |
| [get_FieldName](./get_fieldname/) | Obtiene el nombre de un campo personalizado. |
| [get_Formula](./get_formula/) | Obtiene la fórmula que Microsoft Project usa para rellenar un campo de tarea personalizado. |
| [get_GraphicalIndicator](./get_graphicalindicator/) | Obtiene la información de indicadores gráficos asociada al atributo extendido. Aplicable al formato MPP. |
| [get_Guid](./get_guid/) | Obtiene el GUID de un campo personalizado. |
| [get_LookupUid](./get_lookupuid/) | Obtiene un GUID de la tabla de búsqueda asociada a un campo personalizado. |
| [get_MaxMultiValues](./get_maxmultivalues/) | Obtiene el número máximo de valores que puede establecer en una lista de selección. |
| [get_ParentProject](./get_parentproject/) | Obtiene el proyecto principal para la instancia de ExtendedAttributeDefinition. |
| [get_PhoneticsAlias](./get_phoneticsalias/) | Obtiene la pronunciación fonética del alias de un campo personalizado. |
| [get_RestrictValues](./get_restrictvalues/) | Obtiene un valor que indica si los valores del campo personalizado están restringidos a los valores de la ValueList. |
| [get_RollupType](./get_rolluptype/) | Obtiene la forma en que se calculan los acumulados. |
| [get_SecondaryGuid](./get_secondaryguid/) | Obtiene el GUID secundario del atributo extendido. |
| [get_SecondaryPid](./get_secondarypid/) | Obtiene el PID secundario de un campo personalizado. |
| [get_SummaryRowsCalculationType](./get_summaryrowscalculationtype/) | Obtiene el tipo de cálculo del valor del atributo personalizado para filas de resumen. |
| [get_UserDef](./get_userdef/) | Obtiene un valor que indica si un campo personalizado es definido por el usuario. |
| [get_ValueList](./get_valuelist/) | Obtiene la List< Value > ValueList. |
| [get_ValuelistSortOrder](./get_valuelistsortorder/) | Obtiene la forma en que se ordenan las listas de valores. Los valores son: 0=Descendente, 1=Ascendente. |
| [GetHashCode](./gethashcode/) | Devuelve un código hash para la instancia de la clase ExtendedAttributeDefinition. |
| [RemoveLookupValue](./removelookupvalue/) | Elimina un valor de la lista de búsqueda interna. Esta es una forma preferible de manipular la ValueList . |
| [set_Alias](./set_alias/) | Establece el alias de un campo personalizado. |
| [set_AppendNewValues](./set_appendnewvalues/) | Establece un valor que indica si los nuevos valores añadidos a un proyecto se agregan automáticamente a la lista. |
| [set_AutoRollDown](./set_autorolldown/) | Establece un valor que indica si se habilita un desplazamiento automático a las asignaciones. |
| [set_CalculationType](./set_calculationtype/) | Establece el tipo de cálculo del valor del atributo personalizado. |
| [set_Default](./set_default/) | Establece el valor predeterminado en la lista. |
| [set_DefaultGuid](./set_defaultguid/) | Establece el Guid de la entrada predeterminada de la tabla de búsqueda. |
| [set_ElementType](./set_elementtype/) | Establece que el atributo extendido está asociado a una tarea, un recurso o una asignación. |
| [set_FieldId](./set_fieldid/) | Establece que corresponde al ID de proyecto de un campo personalizado. Utilice la representación en cadena de una constante de la clase Aspose::Tasks::ExtendedAttributeTask para especificar la propiedad FieldId. |
| [set_Formula](./set_formula/) | Establece la fórmula que Microsoft Project utiliza para rellenar un campo de tarea personalizado. |
| [set_GraphicalIndicator](./set_graphicalindicator/) | Establece información de indicadores gráficos asociada al atributo extendido. Aplicable al formato MPP. |
| [set_Guid](./set_guid/) | Establece el Guid de un campo personalizado. |
| [set_MaxMultiValues](./set_maxmultivalues/) | Establece el número máximo de valores que puede establecer en una lista de selección. |
| [set_PhoneticsAlias](./set_phoneticsalias/) | Establece la pronunciación fonética del alias de un campo personalizado. |
| [set_RestrictValues](./set_restrictvalues/) | Establece un valor que indica si los valores del campo personalizado están restringidos a los valores de la ValueList . |
| [set_RollupType](./set_rolluptype/) | Establece la forma en que se calculan los rollups. |
| [set_SecondaryGuid](./set_secondaryguid/) | Establece el guid secundario del atributo extendido. |
| [set_SecondaryPid](./set_secondarypid/) | Establece el PID secundario de un campo personalizado. |
| [set_SummaryRowsCalculationType](./set_summaryrowscalculationtype/) | Establece el tipo de cálculo del valor del atributo personalizado para filas de resumen. |
| [set_UserDef](./set_userdef/) | Establece un valor que indica si un campo personalizado es definido por el usuario. |
| [set_ValuelistSortOrder](./set_valuelistsortorder/) | Establece la forma en que se ordenan las listas de valores. Los valores son: 0=Descendente, 1=Ascendente. |

