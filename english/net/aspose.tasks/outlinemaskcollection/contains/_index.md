---
title: OutlineMaskCollection.Contains
second_title: Aspose.Tasks for .NET API Reference
description: OutlineMaskCollection method. Returns true if the specified item is found in this collection otherwise false
type: docs
weight: 60
url: /net/aspose.tasks/outlinemaskcollection/contains/
---
## OutlineMaskCollection.Contains method

Returns true if the specified item is found in this collection; otherwise, false.

```csharp
public bool Contains(OutlineMask item)
```

| Parameter | Type | Description |
| --- | --- | --- |
| item | OutlineMask | the specified item to find. |

### Return Value

true if the specified item is found in this collection; otherwise, false.

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


