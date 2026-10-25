---
title: "OutlineMaskCollection.Contains"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método de OutlineMaskCollection. Devuelve true si el elemento especificado se encuentra en esta colección, de lo contrario false"
type: docs
weight: 60
url: /es/net/aspose.tasks/outlinemaskcollection/contains/
---
## OutlineMaskCollection.Contains method

Devuelve true si el elemento especificado se encuentra en esta colección; de lo contrario, false.

```csharp
public bool Contains(OutlineMask item)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| elemento | OutlineMask | el elemento especificado para buscar. |

### Valor devuelto

true si el elemento especificado se encuentra en esta colección; de lo contrario, false.

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

* class [OutlineMask](../../outlinemask/)
* class [OutlineMaskCollection](../)
* namespace [Aspose.Tasks](../../outlinemaskcollection/)
* assembly [Aspose.Tasks](../../../)


