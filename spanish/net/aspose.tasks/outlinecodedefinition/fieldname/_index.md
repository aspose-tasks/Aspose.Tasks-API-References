---
title: "OutlineCodeDefinition.FieldName"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "OutlineCodeDefinition propiedad. Obtiene o establece el nombre de un código de esquema personalizado"
type: docs
weight: 70
url: /es/net/aspose.tasks/outlinecodedefinition/fieldname/
---
## OutlineCodeDefinition.FieldName property

Obtiene o establece el nombre de un código de esquema personalizado.

```csharp
public string FieldName { get; set; }
```

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

* class [OutlineCodeDefinition](../)
* namespace [Aspose.Tasks](../../outlinecodedefinition/)
* assembly [Aspose.Tasks](../../../)


