---
title: "OutlineMaskCollection.CopyTo"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος OutlineMaskCollection. Αντιγράφει τα στοιχεία αυτής της συλλογής στον καθορισμένο πίνακα ξεκινώντας από την καθορισμένη θέση του πίνακα"
type: docs
weight: 70
url: /el/net/aspose.tasks/outlinemaskcollection/copyto/
---
## OutlineMaskCollection.CopyTo method

Αντιγράφει τα στοιχεία αυτής της συλλογής στον καθορισμένο πίνακα, ξεκινώντας από τη συγκεκριμένη θέση του πίνακα.

```csharp
public void CopyTo(OutlineMask[] array, int arrayIndex)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| array | OutlineMask[] | ο καθορισμένος μονοδιάστατος πίνακας για αντιγραφή των στοιχείων σε αυτόν |
| arrayIndex | Int32 | ο μηδενικός δείκτης του καθορισμένου πίνακα στον οποίο αρχίζει η αντιγραφή. |

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


