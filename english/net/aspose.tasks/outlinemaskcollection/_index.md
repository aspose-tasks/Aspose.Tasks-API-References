---
title: Class OutlineMaskCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.OutlineMaskCollection class. Represents a collection of OutlineMask objects
type: docs
weight: 1190
url: /net/aspose.tasks/outlinemaskcollection/
---
## OutlineMaskCollection class

Represents a collection of [`OutlineMask`](../outlinemask/) objects.

```csharp
public class OutlineMaskCollection : IList<OutlineMask>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/outlinemaskcollection/count/) { get; } | Gets the number of elements contained in this collection. |
| [IsReadOnly](../../aspose.tasks/outlinemaskcollection/isreadonly/) { get; } | Gets a value indicating whether this collection is read-only; otherwise, false. |
| [Item](../../aspose.tasks/outlinemaskcollection/item/) { get; set; } | Returns or sets the element at the specified index. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/outlinemaskcollection/add/)(OutlineMask) | Adds the specified item to this collection. |
| [Clear](../../aspose.tasks/outlinemaskcollection/clear/)() | Removes all items from this collection. |
| [Contains](../../aspose.tasks/outlinemaskcollection/contains/)(OutlineMask) | Returns true if the specified item is found in this collection; otherwise, false. |
| [CopyTo](../../aspose.tasks/outlinemaskcollection/copyto/)(OutlineMask[], int) | Copies the elements of this collection to the specified array, starting at the specified array index. |
| [GetEnumerator](../../aspose.tasks/outlinemaskcollection/getenumerator/)() | Returns an enumerator for this collection. |
| [IndexOf](../../aspose.tasks/outlinemaskcollection/indexof/)(OutlineMask) | Determines the index of the specified item in this collection. |
| [Insert](../../aspose.tasks/outlinemaskcollection/insert/)(int, OutlineMask) | Inserts the specified item at the specified index. |
| [Remove](../../aspose.tasks/outlinemaskcollection/remove/)(OutlineMask) | Removes the first occurrence of a specific object from this collection. |
| [RemoveAt](../../aspose.tasks/outlinemaskcollection/removeat/)(int) | Removes an item at the specified index. |

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

* class [OutlineMask](../outlinemask/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


