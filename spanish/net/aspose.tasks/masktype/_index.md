---
title: "Enum MaskType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.MaskType. Especifica el tipo de una máscara"
type: docs
weight: 1000
url: /es/net/aspose.tasks/masktype/
---
## MaskType enumeration

Especifica el tipo de una máscara.

```csharp
public enum MaskType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Null | `0` | Indica el tipo de máscara Null. |
| Numbers | `1` | Indica el tipo de máscara Numbers. |
| UpperCaseLetters | `2` | Indica el tipo de máscara UpperCaseLetters. |
| LowerCaseLetters | `3` | Indica el tipo de máscara LowerCaseLetters. |
| Characters | `4` | Indica el tipo de máscara Characters. |
| Val4 | `5` | Indica el tipo de máscara Lookup para Cost. |
| Val5 | `6` | Indica el tipo de máscara Lookup para Dates. |
| Val6 | `7` | Indica el tipo de máscara Lookup para Durations. |
| Val7 | `8` | Indica el tipo de máscara Lookup para Numbers. |
| Val8 | `9` | Indica el tipo de máscara Lookup para Flags. |
| Val9 | `10` | Indica el tipo de máscara Lookup para FinishDate. |

## Ejemplos

Muestra cómo trabajar con colecciones de máscaras de contorno.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = project.OutlineCodes[0];

// borrar máscaras de contorno
if (outline.Masks.Count > 0)
{
    if (!outline.Masks.IsReadOnly)
    {
        outline.Masks.Clear();
    }
}

var mask = new OutlineMask();
mask.Type = MaskType.Characters;
var maskWrong = new OutlineMask();
maskWrong.Type = MaskType.Null;

outline.Masks.Add(mask);

// insertar una máscara incorrecta
outline.Masks.Insert(0, maskWrong);

// editar la máscara usando acceso por índice de la colección
var idx = outline.Masks.IndexOf(mask);
outline.Masks[idx].Length = 2;

// eliminar una máscara incorrecta por índice
var idxOfWrong = outline.Masks.IndexOf(maskWrong);
outline.Masks.RemoveAt(idxOfWrong);

// iterar sobre máscaras
foreach (var outlineMask in outline.Masks)
{
    Console.WriteLine("Length: " + outlineMask.Length);
    Console.WriteLine("Level: " + outlineMask.Level);
    Console.WriteLine("Separator: " + outlineMask.Separator);
    Console.WriteLine("Type: " + outlineMask.Type);
}

var otherProject = new Project(DataDir + "OutlineValues2010.mpp");

var otherOutline = otherProject.OutlineCodes[0];

var masks = new OutlineMask[outline.Masks.Count];
outline.Masks.CopyTo(masks, 0);

foreach (var maskToAdd in masks)
{
    if (!otherOutline.Masks.Contains(maskToAdd))
    {
        otherOutline.Masks.Add(maskToAdd);
    }
}
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


