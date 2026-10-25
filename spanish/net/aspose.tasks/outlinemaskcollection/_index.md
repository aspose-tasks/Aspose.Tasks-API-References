---
title: "Clase OutlineMaskCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.OutlineMaskCollection. Representa una colección de objetos OutlineMask"
type: docs
weight: 1200
url: /es/net/aspose.tasks/outlinemaskcollection/
---
## OutlineMaskCollection class

Representa una colección de objetos [`OutlineMask`](../outlinemask/).

```csharp
public class OutlineMaskCollection : IList<OutlineMask>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.tasks/outlinemaskcollection/count/) { get; } | Obtiene el número de elementos contenidos en esta colección. |
| [IsReadOnly](../../aspose.tasks/outlinemaskcollection/isreadonly/) { get; } | Obtiene un valor que indica si esta colección es de solo lectura; de lo contrario, false. |
| [Item](../../aspose.tasks/outlinemaskcollection/item/) { get; set; } | Devuelve o establece el elemento en el índice especificado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.tasks/outlinemaskcollection/add/)(OutlineMask) | Agrega el elemento especificado a esta colección. |
| [Clear](../../aspose.tasks/outlinemaskcollection/clear/)() | Elimina todos los elementos de esta colección. |
| [Contains](../../aspose.tasks/outlinemaskcollection/contains/)(OutlineMask) | Devuelve true si el elemento especificado se encuentra en esta colección; de lo contrario, false. |
| [CopyTo](../../aspose.tasks/outlinemaskcollection/copyto/)(OutlineMask[], int) | Copia los elementos de esta colección al array especificado, comenzando en el índice de array especificado. |
| [GetEnumerator](../../aspose.tasks/outlinemaskcollection/getenumerator/)() | Devuelve un enumerador para esta colección. |
| [IndexOf](../../aspose.tasks/outlinemaskcollection/indexof/)(OutlineMask) | Determina el índice del elemento especificado en esta colección. |
| [Insert](../../aspose.tasks/outlinemaskcollection/insert/)(int, OutlineMask) | Inserta el elemento especificado en el índice especificado. |
| [Remove](../../aspose.tasks/outlinemaskcollection/remove/)(OutlineMask) | Elimina la primera aparición de un objeto específico de esta colección. |
| [RemoveAt](../../aspose.tasks/outlinemaskcollection/removeat/)(int) | Elimina un elemento en el índice especificado. |

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

* class [OutlineMask](../outlinemask/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


