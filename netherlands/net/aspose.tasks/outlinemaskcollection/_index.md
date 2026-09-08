---
title: "Klasse OutlineMaskCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.OutlineMaskCollection class. Vertegenwoordigt een collectie van OutlineMask-objecten"
type: docs
weight: 1200
url: /nl/net/aspose.tasks/outlinemaskcollection/
---
## OutlineMaskCollection class

Vertegenwoordigt een collectie van [`OutlineMask`](../outlinemask/) objecten.

```csharp
public class OutlineMaskCollection : IList<OutlineMask>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks/outlinemaskcollection/count/) { get; } | Haalt het aantal elementen op dat in deze collectie zit. |
| [IsReadOnly](../../aspose.tasks/outlinemaskcollection/isreadonly/) { get; } | Haalt een waarde op die aangeeft of deze collectie alleen-lezen is; anders, false. |
| [Item](../../aspose.tasks/outlinemaskcollection/item/) { get; set; } | Retourneert of stelt het element in op de opgegeven index. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../aspose.tasks/outlinemaskcollection/add/)(OutlineMask) | Voegt het opgegeven item toe aan deze collectie. |
| [Clear](../../aspose.tasks/outlinemaskcollection/clear/)() | Verwijdert alle items uit deze collectie. |
| [Contains](../../aspose.tasks/outlinemaskcollection/contains/)(OutlineMask) | Retourneert true als het opgegeven item in deze collectie wordt gevonden; anders false. |
| [CopyTo](../../aspose.tasks/outlinemaskcollection/copyto/)(OutlineMask[], int) | Kopieert de elementen van deze collectie naar de opgegeven array, beginnend bij de opgegeven array-index. |
| [GetEnumerator](../../aspose.tasks/outlinemaskcollection/getenumerator/)() | Retourneert een enumerator voor deze collectie. |
| [IndexOf](../../aspose.tasks/outlinemaskcollection/indexof/)(OutlineMask) | Bepaalt de index van het opgegeven item in deze collectie. |
| [Insert](../../aspose.tasks/outlinemaskcollection/insert/)(int, OutlineMask) | Voegt het opgegeven item in op de opgegeven index. |
| [Remove](../../aspose.tasks/outlinemaskcollection/remove/)(OutlineMask) | Verwijdert de eerste instantie van een specifiek object uit deze collectie. |
| [RemoveAt](../../aspose.tasks/outlinemaskcollection/removeat/)(int) | Verwijdert een item op de opgegeven index. |

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

* class [OutlineMask](../outlinemask/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


