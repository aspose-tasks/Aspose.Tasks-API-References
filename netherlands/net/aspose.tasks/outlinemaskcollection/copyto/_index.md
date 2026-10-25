---
title: "OutlineMaskCollection.CopyTo"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "OutlineMaskCollection methode. Kopieert de elementen van deze collectie naar de opgegeven array, beginnend bij de opgegeven array-index"
type: docs
weight: 70
url: /nl/net/aspose.tasks/outlinemaskcollection/copyto/
---
## OutlineMaskCollection.CopyTo method

Kopieert de elementen van deze collectie naar de opgegeven array, beginnend bij de opgegeven array-index.

```csharp
public void CopyTo(OutlineMask[] array, int arrayIndex)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| array | OutlineMask[] | de opgegeven eendimensionale array om elementen naartoe te kopiëren |
| arrayIndex | Int32 | de nulgebaseerde index van de opgegeven array waarop het kopiëren begint. |

## Voorbeelden

Toont hoe te werken met outline-maskerverzamelingen.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = project.OutlineCodes[0];

// outline-masks wissen
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

// Voeg een onjuiste masker in.
outline.Masks.Insert(0, maskWrong);

// bewerk het masker door indextoegang van de collectie te gebruiken
var idx = outline.Masks.IndexOf(mask);
outline.Masks[idx].Length = 2;

// verwijder een onjuiste masker op index
var idxOfWrong = outline.Masks.IndexOf(maskWrong);
outline.Masks.RemoveAt(idxOfWrong);

// itereren over maskers
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

### Zie ook

* class [OutlineMask](../../outlinemask/)
* class [OutlineMaskCollection](../)
* namespace [Aspose.Tasks](../../outlinemaskcollection/)
* assembly [Aspose.Tasks](../../../)


