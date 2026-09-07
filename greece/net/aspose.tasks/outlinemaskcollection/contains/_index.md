---
title: "OutlineMaskCollection.Contains"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "OutlineMaskCollection μέθοδος. Επιστρέφει true εάν το καθορισμένο στοιχείο βρεθεί σε αυτή τη συλλογή, διαφορετικά false"
type: docs
weight: 60
url: /el/net/aspose.tasks/outlinemaskcollection/contains/
---
## OutlineMaskCollection.Contains method

Επιστρέφει true εάν το καθορισμένο στοιχείο βρεθεί σε αυτή τη συλλογή· διαφορετικά, false.

```csharp
public bool Contains(OutlineMask item)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| item | OutlineMask | το καθορισμένο στοιχείο για εύρεση. |

### Τιμή Επιστροφής

αληθές εάν το καθορισμένο στοιχείο βρεθεί σε αυτή τη συλλογή· διαφορετικά, ψευδές.

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


