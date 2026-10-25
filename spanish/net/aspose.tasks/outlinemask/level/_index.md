---
title: "OutlineMask.Level"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad OutlineMask. Obtiene o establece el nivel de una máscara"
type: docs
weight: 30
url: /es/net/aspose.tasks/outlinemask/level/
---
## OutlineMask.Level property

Obtiene o establece el nivel de una máscara.

```csharp
public int Level { get; set; }
```

## Ejemplos

Muestra cómo trabajar con máscaras de esquema.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = new OutlineCodeDefinition();
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline.Alias = "My Outline Code";

project.OutlineCodes.Add(outline);

var mask = new OutlineMask();

// establece el tipo de una máscara
mask.Type = MaskType.Characters;

// establece el separador de los valores de código
mask.Separator = "/";

// establece el nivel de una máscara
mask.Level = 1;

// establece la longitud máxima (en caracteres) de los valores de código de esquema. 0 si la longitud no está definida.
mask.Length = 2;

// agrega la máscara a la definición
outline.Masks.Add(mask);

var value = new OutlineValue();
value.Value = "Text value 1";
value.ValueId = 1;
value.Type = OutlineValueType.Text;
value.Description = "Text value descr 1";
outline.Values.Add(value);

// ...
```

### Ver también

* class [OutlineMask](../)
* namespace [Aspose.Tasks](../../outlinemask/)
* assembly [Aspose.Tasks](../../../)


