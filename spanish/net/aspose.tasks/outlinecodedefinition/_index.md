---
title: "Clase OutlineCodeDefinition"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.OutlineCodeDefinition. Representa una definición de código de esquema."
type: docs
weight: 1170
url: /es/net/aspose.tasks/outlinecodedefinition/
---
## OutlineCodeDefinition class

Representa una definición de código de esquema.

```csharp
public sealed class OutlineCodeDefinition
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [OutlineCodeDefinition](outlinecodedefinition/)() | Inicializa una nueva instancia de la clase `OutlineCodeDefinition`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Alias](../../aspose.tasks/outlinecodedefinition/alias/) { get; set; } | Obtiene o establece el alias de un código de esquema personalizado. |
| [AllLevelsRequired](../../aspose.tasks/outlinecodedefinition/alllevelsrequired/) { get; set; } | Obtiene o establece un valor que indica si los nuevos códigos deben tener todos los niveles. No disponible para códigos empresariales. |
| [Enterprise](../../aspose.tasks/outlinecodedefinition/enterprise/) { get; set; } | Obtiene o establece un valor que indica si un código de esquema personalizado es un código de esquema empresarial personalizado. |
| [EnterpriseOutlineCodeAlias](../../aspose.tasks/outlinecodedefinition/enterpriseoutlinecodealias/) { get; set; } | Obtiene o establece una referencia a otro campo personalizado para el cual esta definición de código de esquema es un alias. |
| [FieldId](../../aspose.tasks/outlinecodedefinition/fieldid/) { get; set; } | Obtiene o establece el número de campo de un código de esquema. |
| [FieldName](../../aspose.tasks/outlinecodedefinition/fieldname/) { get; set; } | Obtiene o establece el nombre de un código de esquema personalizado. |
| [Guid](../../aspose.tasks/outlinecodedefinition/guid/) { get; set; } | Obtiene o establece el GUID de un código de esquema. |
| [LeafOnly](../../aspose.tasks/outlinecodedefinition/leafonly/) { get; set; } | Obtiene o establece un valor que indica si los valores especificados en este campo de código de esquema deben ser valores hoja. |
| [Masks](../../aspose.tasks/outlinecodedefinition/masks/) { get; } | Obtiene el objeto OutlineMaskCollection. La tabla de entradas que define la máscara del código de esquema. Instancia de solo lectura [`OutlineMaskCollection`](../outlinemaskcollection/). |
| [OnlyTableValuesAllowed](../../aspose.tasks/outlinecodedefinition/onlytablevaluesallowed/) { get; set; } | Obtiene o establece un valor que indica si los valores especificados deben provenir de la tabla de valores. |
| [PhoneticAlias](../../aspose.tasks/outlinecodedefinition/phoneticalias/) { get; set; } | Obtiene o establece la pronunciación fonética del alias del código de esquema personalizado. |
| [ResourceSubstitutionEnabled](../../aspose.tasks/outlinecodedefinition/resourcesubstitutionenabled/) { get; set; } | Obtiene o establece un valor que indica si el código de esquema personalizado puede ser usado por el Asistente de sustitución de recursos en Microsoft Project. |
| [ShowIndent](../../aspose.tasks/outlinecodedefinition/showindent/) { get; set; } | Obtiene o establece un valor que indica si los sangrados de este código de esquema deben mostrarse. |
| [Values](../../aspose.tasks/outlinecodedefinition/values/) { get; } | Obtiene el objeto OutlineValueCollection. Los valores de la tabla asociados con este código de esquema. |

## Ejemplos

Muestra cómo trabajar con definiciones de códigos de esquema.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// crear una nueva definición de código de esquema
var outline = new OutlineCodeDefinition();

// establecer el número de campo de un código de esquema
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");

// establecer el nombre de un código de esquema personalizado
outline.FieldName = "Outline Code1";

// establecer el Guid de un código de esquema
outline.Guid = "e6afac06-0d86-4359-a96c-db705e3d2ca8";

// establecer un valor que indique si los valores especificados en este campo de código de esquema deben ser valores hoja
outline.LeafOnly = false;

// establecer el alias de un código de esquema personalizado
outline.Alias = "My Outline Code";

// establecer la pronunciación fonética del alias del código de esquema personalizado
outline.PhoneticAlias = "Outline Code";

// establecer un valor que indique si los códigos nuevos deben tener todos los niveles. No disponible para Códigos Empresariales.
outline.AllLevelsRequired = true;

// establecer un valor que indique si un código de esquema personalizado es un código de esquema empresarial personalizado
outline.Enterprise = false;

// establecer una referencia a otro campo personalizado para el cual esta definición de código de esquema es un alias
outline.EnterpriseOutlineCodeAlias = 0;

// agregar una máscara de esquema
var mask = new OutlineMask();
mask.Type = MaskType.Characters;
outline.Masks.Add(mask);

// establecer un valor que indique si los valores especificados deben provenir de la tabla de valores
outline.OnlyTableValuesAllowed = false;

// establecer un valor que indique si el código de esquema personalizado puede ser utilizado
// por el Asistente de Sustitución de Recursos en Microsoft Project
outline.ResourceSubstitutionEnabled = false;

// establecer un valor que indique si los sangrados de este código de esquema deben mostrarse.
outline.ShowIndent = false;

project.OutlineCodes.Add(outline);

var value = new OutlineValue();
value.Value = "Text value 1";
value.ValueId = 1;
value.Type = OutlineValueType.Text;
value.Description = "Text value descr 1";
outline.Values.Add(value);

// ...
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


