---
title: ExtendedAttributeDefinition
second_title: Referencia de Aspose.Tasks para la API de .NET
description: Representa una definición de atributo extendida asociada con un proyecto.
type: docs
weight: 530
url: /es/net/aspose.tasks/extendedattributedefinition/
---
## ExtendedAttributeDefinition class

Representa una definición de atributo extendida asociada con un proyecto.

```csharp
public class ExtendedAttributeDefinition
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Alias](../../aspose.tasks/extendedattributedefinition/alias) { get; set; } | Obtiene o establece el alias de un campo personalizado. |
| [AppendNewValues](../../aspose.tasks/extendedattributedefinition/appendnewvalues) { get; set; } | Obtiene o establece un valor que indica si los nuevos valores agregados a un proyecto se agregan automáticamente a la lista. |
| [AutoRollDown](../../aspose.tasks/extendedattributedefinition/autorolldown) { get; set; } | Obtiene o establece un valor que indica si está habilitada una reducción automática a las asignaciones. |
| [CalculationType](../../aspose.tasks/extendedattributedefinition/calculationtype) { get; set; } | Obtiene o establece el tipo de cálculo del valor del atributo personalizado. |
| [CfType](../../aspose.tasks/extendedattributedefinition/cftype) { get; } | Obtiene el tipo de un campo personalizado. |
| [Default](../../aspose.tasks/extendedattributedefinition/default) { get; set; } | Obtiene o establece el valor predeterminado en la lista. |
| [DefaultGuid](../../aspose.tasks/extendedattributedefinition/defaultguid) { get; set; } | Obtiene o establece el Guid de la entrada de la tabla de búsqueda predeterminada. |
| [ElementType](../../aspose.tasks/extendedattributedefinition/elementtype) { get; set; } | Obtiene o establece el atributo extendido asociado a una tarea, recurso o asignación. |
| [FieldId](../../aspose.tasks/extendedattributedefinition/fieldid) { get; set; } | Obtiene o establece la identificación del proyecto de un campo personalizado. Usar la representación de cadena de una constante de[`ExtendedAttributeTask`](../extendedattributetask) clase para especificar[`FieldId`](./fieldid) propiedad. |
| [FieldName](../../aspose.tasks/extendedattributedefinition/fieldname) { get; } | Obtiene el nombre de un campo personalizado. |
| [Formula](../../aspose.tasks/extendedattributedefinition/formula) { get; set; } | Obtiene o establece la fórmula que usa Microsoft Project para completar un campo de tarea personalizado. |
| [Guid](../../aspose.tasks/extendedattributedefinition/guid) { get; set; } | Obtiene o establece el Guid de un campo personalizado. |
| [LookupUid](../../aspose.tasks/extendedattributedefinition/lookupuid) { get; } | Obtiene un Guid de la tabla de búsqueda asociada con un campo personalizado. |
| [MaxMultiValues](../../aspose.tasks/extendedattributedefinition/maxmultivalues) { get; set; } | Obtiene o establece el número máximo de valores que puede establecer en una lista de selección. |
| [ParentProject](../../aspose.tasks/extendedattributedefinition/parentproject) { get; } | Obtiene el proyecto padre para el[`ExtendedAttributeDefinition`](../extendedattributedefinition) instancia. |
| [PhoneticsAlias](../../aspose.tasks/extendedattributedefinition/phoneticsalias) { get; set; } | Obtiene o establece la pronunciación fonética del alias de un campo personalizado. |
| [RestrictValues](../../aspose.tasks/extendedattributedefinition/restrictvalues) { get; set; } | Obtiene o establece un valor que indica si los valores del campo personalizado están restringidos a los valores del[`ValueList`](./valuelist) . |
| [RollupType](../../aspose.tasks/extendedattributedefinition/rolluptype) { get; set; } | Obtiene o establece la forma en que se calculan los rollups. |
| [SecondaryGuid](../../aspose.tasks/extendedattributedefinition/secondaryguid) { get; set; } | Obtiene o establece el GUID secundario del atributo extendido. |
| [SecondaryPid](../../aspose.tasks/extendedattributedefinition/secondarypid) { get; set; } | Obtiene o establece el PID secundario de un campo personalizado. |
| [SummaryRowsCalculationType](../../aspose.tasks/extendedattributedefinition/summaryrowscalculationtype) { get; set; } | Obtiene o establece el tipo de cálculo del valor del atributo personalizado para las filas de resumen. |
| [UserDef](../../aspose.tasks/extendedattributedefinition/userdef) { get; set; } | Obtiene o establece un valor que indica si un campo personalizado está definido por el usuario. |
| [ValueList](../../aspose.tasks/extendedattributedefinition/valuelist) { get; } | Obtiene List&lt;Value&gt; ValueList. |
| [ValuelistSortOrder](../../aspose.tasks/extendedattributedefinition/valuelistsortorder) { get; set; } | Obtiene o establece la forma en que se ordenan las listas de valores. Los valores son: 0=Descendente, 1=Ascendente. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition#createlookupresourcedefinition_1)(ExtendedAttributeResource, string) | Método de fábrica que crea una definición de atributo extendida con búsqueda. Tiene[`CalculationType`](./calculationtype) igual aLookup y solo se puede usar en Recursos. Debe especificar*fieldId* y*alias* cuando llame a este método. El tipo de campo se deduce del campo id. |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition#createlookupresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Método de fábrica que crea una definición de atributo extendida con búsqueda. Tiene[`CalculationType`](./calculationtype) igual aLookup y solo se puede usar en Recursos. Debe especificar*customFieldType* ,*fieldId* y*alias* cuando llame a este método. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition#createlookuptaskdefinition_1)(ExtendedAttributeTask, string) | Método de fábrica que crea una definición de atributo extendida con búsqueda. Tiene[`CalculationType`](./calculationtype) igual aLookup y solo se puede usar en Tareas. Debe especificar*fieldId* y*alias* cuando llame a este método. El tipo de campo se deduce del campo id. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition#createlookuptaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Método de fábrica que crea una definición de atributo extendida con búsqueda. Tiene[`CalculationType`](./calculationtype) igual aLookup y solo se puede usar en Tareas. Debe especificar*customFieldType* ,*fieldId* y*alias* cuando llame a este método. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition#createresourcedefinition_1)(ExtendedAttributeResource, string) | Método de fábrica que crea una definición de atributo extendida simple, que Microsoft Project muestra como "Ninguno". Tiene[`CalculationType`](./calculationtype) igual aNone y solo se puede usar en Recurso. Debe especificar*fieldId* y*alias* cuando llame a este método. El tipo de campo se deduce del campo id. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition#createresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Método de fábrica que crea una definición de atributo extendida simple, que Microsoft Project muestra como "Ninguno". Tiene[`CalculationType`](./calculationtype) igual aNone y solo se puede usar en Recurso. Debe especificar*customFieldType* ,*fieldId* y*alias* cuando llame a este método. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition#createtaskdefinition_1)(ExtendedAttributeTask, string) | Método de fábrica que crea una definición de atributo extendida simple, que Microsoft Project muestra como "Ninguno". Tiene[`CalculationType`](./calculationtype) igual aNone y solo se puede usar en Tareas. Debe especificar*fieldId* y*alias* al llamar a este método. El tipo de campo se deduce del campo id. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition#createtaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Método de fábrica que crea una definición de atributo extendida simple, que Microsoft Project muestra como "Ninguno". Tiene[`CalculationType`](./calculationtype) igual aNone y solo se puede usar en Tareas. Debe especificar*customFieldType* ,*fieldId* y*alias* al llamar a este método. |
| [AddLookupValue](../../aspose.tasks/extendedattributedefinition/addlookupvalue)(Value) | Agrega un valor a la lista de búsqueda interna. Esta es una forma preferible para las manipulaciones con el[`ValueList`](./valuelist) . |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute)() | Crea un nuevo atributo extendido con el ID de campo que es igual al valor de ID de campo de este objeto. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_3)(bool) | Crea un nuevo atributo extendido con el Id. de campo que es igual al valor de Id. de campo de este objeto y el valor de indicador especificado. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_4)(DateTime) | Crea un nuevo atributo extendido con el Id. de campo que es igual al valor de Id. de campo de este objeto y el valor de fecha especificado. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_5)(decimal) | Crea un nuevo atributo extendido con el ID de campo que es igual al valor de ID de campo de este objeto y el valor numérico especificado. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_1)(Duration) | Crea un nuevo atributo extendido con el Id. de campo que es igual al valor de Id. de campo de este objeto y el valor de duración especificado. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_6)(string) | Crea un nuevo atributo extendido con el ID de campo que es igual al valor de ID de campo de este objeto y el valor de texto especificado. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_2)(Value) | Crea un nuevo atributo extendido vinculado con el especificado[`Value`](../value) artículo. |
| override [Equals](../../aspose.tasks/extendedattributedefinition/equals)(object) | Devuelve un indicador que indica si esta instancia es igual al objeto especificado. |
| override [GetHashCode](../../aspose.tasks/extendedattributedefinition/gethashcode)() | Devuelve un código hash para la instancia del[`ExtendedAttributeDefinition`](../extendedattributedefinition) clase. |
| [RemoveLookupValue](../../aspose.tasks/extendedattributedefinition/removelookupvalue)(Value) | Elimina un valor de la lista de búsqueda interna. Esta es una forma preferible para las manipulaciones con el[`ValueList`](./valuelist) . |

### Ver también

* espacio de nombres [Aspose.Tasks](../../aspose.tasks)
* asamblea [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
