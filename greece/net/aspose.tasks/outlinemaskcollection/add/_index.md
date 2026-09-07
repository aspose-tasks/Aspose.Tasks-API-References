---
title: "OutlineMaskCollection.Add"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος OutlineMaskCollection. Προσθέτει το καθορισμένο στοιχείο σε αυτή τη συλλογή"
type: docs
weight: 40
url: /el/net/aspose.tasks/outlinemaskcollection/add/
---
## OutlineMaskCollection.Add method

Προσθέτει το καθορισμένο στοιχείο σε αυτή τη συλλογή.

```csharp
public void Add(OutlineMask item)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| item | OutlineMask | το καθορισμένο στοιχείο για προσθήκη σε αυτή τη συλλογή. |

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

* class [OutlineMask](../../outlinemask/)
* class [OutlineMaskCollection](../)
* namespace [Aspose.Tasks](../../outlinemaskcollection/)
* assembly [Aspose.Tasks](../../../)


