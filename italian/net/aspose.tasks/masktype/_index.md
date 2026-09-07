---
title: "Enum MaskType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.MaskType. Specifica il tipo di una maschera."
type: docs
weight: 1000
url: /it/net/aspose.tasks/masktype/
---
## MaskType enumeration

Specifica il tipo di maschera.

```csharp
public enum MaskType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Null | `0` | Indica il tipo di maschera Null. |
| Numbers | `1` | Indica il tipo di maschera Numbers. |
| UpperCaseLetters | `2` | Indica il tipo di maschera UpperCaseLetters. |
| LowerCaseLetters | `3` | Indica il tipo di maschera LowerCaseLetters. |
| Characters | `4` | Indica il tipo di maschera Characters. |
| Val4 | `5` | Indica il tipo di maschera Lookup per Cost. |
| Val5 | `6` | Indica il tipo di maschera Lookup per Dates. |
| Val6 | `7` | Indica il tipo di maschera Lookup per Durations. |
| Val7 | `8` | Indica il tipo di maschera Lookup per Numbers. |
| Val8 | `9` | Indica il tipo di maschera Lookup per Flags. |
| Val9 | `10` | Indica il tipo di maschera Lookup per FinishDate. |

## Esempi

Mostra come lavorare con le raccolte di maschere outline.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = project.OutlineCodes[0];

// cancella le maschere outline
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

// inserisci una maschera errata
outline.Masks.Insert(0, maskWrong);

// modifica la maschera usando l'accesso per indice della raccolta
var idx = outline.Masks.IndexOf(mask);
outline.Masks[idx].Length = 2;

// rimuovi una maschera errata per indice
var idxOfWrong = outline.Masks.IndexOf(maskWrong);
outline.Masks.RemoveAt(idxOfWrong);

// itera sulle maschere
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

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


