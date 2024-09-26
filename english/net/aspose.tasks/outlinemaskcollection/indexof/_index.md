---
title: OutlineMaskCollection.IndexOf
second_title: Aspose.Tasks for .NET API Reference
description: OutlineMaskCollection method. Determines the index of the specified item in this collection
type: docs
weight: 90
url: /net/aspose.tasks/outlinemaskcollection/indexof/
---
## OutlineMaskCollection.IndexOf method

Determines the index of the specified item in this collection.

```csharp
public int IndexOf(OutlineMask item)
```

| Parameter | Type | Description |
| --- | --- | --- |
| item | OutlineMask | the specified item to locate in this collection. |

### Return Value

the index of the specified item if found; otherwise, -1.

## Examples

Shows how to work with outline mask collections.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = project.OutlineCodes[0];

// clear outline masks
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

// insert a wrong mask 
outline.Masks.Insert(0, maskWrong);

// edit the mask by using index access of collection
var idx = outline.Masks.IndexOf(mask);
outline.Masks[idx].Length = 2;

// remove a wrong mask by index
var idxOfWrong = outline.Masks.IndexOf(maskWrong);
outline.Masks.RemoveAt(idxOfWrong);

// iterate over masks
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

### See Also

* class [OutlineMask](../../outlinemask/)
* class [OutlineMaskCollection](../)
* namespace [Aspose.Tasks](../../outlinemaskcollection/)
* assembly [Aspose.Tasks](../../../)


