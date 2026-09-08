---
title: "Clase OutlineMask"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.OutlineMask. Representa cuatro elementos de una máscara que define un formato de código de esquema"
type: docs
weight: 1190
url: /es/net/aspose.tasks/outlinemask/
---
## OutlineMask class

Representa cuatro elementos de una máscara que define un formato de código de esquema.

```csharp
public class OutlineMask
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [OutlineMask](outlinemask/)() | Inicializa una nueva instancia de la clase `OutlineMask`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Length](../../aspose.tasks/outlinemask/length/) { get; set; } | Obtiene o establece la longitud máxima (en caracteres) de los valores del código de esquema. 0 si la longitud no está definida. |
| [Level](../../aspose.tasks/outlinemask/level/) { get; set; } | Obtiene o establece el nivel de una máscara. |
| [Separator](../../aspose.tasks/outlinemask/separator/) { get; set; } | Obtiene o establece el separador de los valores de código. |
| [Type](../../aspose.tasks/outlinemask/type/) { get; set; } | Obtiene o establece el tipo de una máscara. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


