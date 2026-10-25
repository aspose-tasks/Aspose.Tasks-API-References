---
title: "Enum MaskType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.MaskType enum. Spécifie le type d'un masque"
type: docs
weight: 1000
url: /fr/net/aspose.tasks/masktype/
---
## MaskType enumeration

Spécifie le type d'un masque.

```csharp
public enum MaskType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Null | `0` | Indique le type de masque Null. |
| Numbers | `1` | Indique le type de masque Numbers. |
| UpperCaseLetters | `2` | Indique le type de masque UpperCaseLetters. |
| LowerCaseLetters | `3` | Indique le type de masque LowerCaseLetters. |
| Characters | `4` | Indique le type de masque Characters. |
| Val4 | `5` | Indique le type de masque Lookup for Cost. |
| Val5 | `6` | Indique le type de masque Lookup for Dates. |
| Val6 | `7` | Indique le type de masque Lookup for Durations. |
| Val7 | `8` | Indique le type de masque Lookup for Numbers. |
| Val8 | `9` | Indique le type de masque Lookup for Flags. |
| Val9 | `10` | Indique le type de masque Lookup for FinishDate. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


