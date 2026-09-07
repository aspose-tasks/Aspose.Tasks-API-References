---
title: "Απαρίθμηση MaskType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Απαρίθμηση Aspose.Tasks.MaskType. Καθορίζει τον τύπο μιας μάσκας"
type: docs
weight: 1000
url: /el/net/aspose.tasks/masktype/
---
## MaskType enumeration

Καθορίζει τον τύπο μιας μάσκας.

```csharp
public enum MaskType
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Null | `0` | Δείχνει τον τύπο μάσκας Null. |
| Numbers | `1` | Δείχνει τον τύπο μάσκας Numbers. |
| UpperCaseLetters | `2` | Δείχνει τον τύπο μάσκας UpperCaseLetters. |
| LowerCaseLetters | `3` | Δείχνει τον τύπο μάσκας LowerCaseLetters. |
| Characters | `4` | Δείχνει τον τύπο μάσκας Characters. |
| Val4 | `5` | Δείχνει την αναζήτηση για τύπο μάσκας Cost. |
| Val5 | `6` | Δείχνει την αναζήτηση για τύπο μάσκας Dates. |
| Val6 | `7` | Δείχνει την αναζήτηση για τύπο μάσκας Durations. |
| Val7 | `8` | Δείχνει την αναζήτηση για τύπο μάσκας Numbers. |
| Val8 | `9` | Δείχνει την αναζήτηση για τύπο μάσκας Flags. |
| Val9 | `10` | Δείχνει την αναζήτηση για τύπο μάσκας FinishDate. |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με συλλογές μάσκας περιγράμματος.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = project.OutlineCodes[0];

// καθαρισμός μάσκων περιγράμματος
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

// εισάγετε μια λανθασμένη μάσκα
outline.Masks.Insert(0, maskWrong);

// επεξεργαστείτε τη μάσκα χρησιμοποιώντας πρόσβαση με δείκτη στη συλλογή
var idx = outline.Masks.IndexOf(mask);
outline.Masks[idx].Length = 2;

// αφαιρέστε μια λανθασμένη μάσκα με δείκτη
var idxOfWrong = outline.Masks.IndexOf(maskWrong);
outline.Masks.RemoveAt(idxOfWrong);

// επανάληψη στις μάσκες
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

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


