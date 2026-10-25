---
title: "OutlineMaskCollection.CopyTo"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "OutlineMaskCollection method. Copie les éléments de cette collection dans le tableau spécifié en commençant à l'index de tableau indiqué"
type: docs
weight: 70
url: /fr/net/aspose.tasks/outlinemaskcollection/copyto/
---
## OutlineMaskCollection.CopyTo method

Copie les éléments de cette collection dans le tableau spécifié, en commençant à l'index de tableau spécifié.

```csharp
public void CopyTo(OutlineMask[] array, int arrayIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| tableau | OutlineMask[] | le tableau unidimensionnel spécifié dans lequel copier les éléments |
| arrayIndex | Int32 | l'index zéro basé du tableau spécifié à partir duquel la copie commence. |

## Exemples

Montre comment travailler avec des collections de masques de contour.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = project.OutlineCodes[0];

// effacer les masques de contour
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

// insérer un masque incorrect
outline.Masks.Insert(0, maskWrong);

// modifier le masque en utilisant l'accès par index de la collection
var idx = outline.Masks.IndexOf(mask);
outline.Masks[idx].Length = 2;

// supprimer un masque incorrect par index
var idxOfWrong = outline.Masks.IndexOf(maskWrong);
outline.Masks.RemoveAt(idxOfWrong);

// itérer sur les masques
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

### Voir aussi

* class [OutlineMask](../../outlinemask/)
* class [OutlineMaskCollection](../)
* namespace [Aspose.Tasks](../../outlinemaskcollection/)
* assembly [Aspose.Tasks](../../../)


