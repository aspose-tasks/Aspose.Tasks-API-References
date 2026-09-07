---
title: "OutlineMaskCollection.Count"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà OutlineMaskCollection. Ottiene il numero di elementi contenuti in questa collezione"
type: docs
weight: 10
url: /it/net/aspose.tasks/outlinemaskcollection/count/
---
## OutlineMaskCollection.Count property

Ottiene il numero di elementi contenuti in questa collezione.

```csharp
public int Count { get; }
```

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

* class [OutlineMaskCollection](../)
* namespace [Aspose.Tasks](../../outlinemaskcollection/)
* assembly [Aspose.Tasks](../../../)


