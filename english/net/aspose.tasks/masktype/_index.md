---
title: Enum MaskType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.MaskType enum. Specifies the type of a mask
type: docs
weight: 990
url: /net/aspose.tasks/masktype/
---
## MaskType enumeration

Specifies the type of a mask.

```csharp
public enum MaskType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Null | `0` | Indicates Null mask type. |
| Numbers | `1` | Indicates Numbers mask type. |
| UpperCaseLetters | `2` | Indicates UpperCaseLetters mask type. |
| LowerCaseLetters | `3` | Indicates LowerCaseLetters mask type. |
| Characters | `4` | Indicates Characters mask type. |
| Val4 | `5` | Indicates Lookup for Cost mask type. |
| Val5 | `6` | Indicates Lookup for Dates mask type. |
| Val6 | `7` | Indicates Lookup for Durations mask type. |
| Val7 | `8` | Indicates Lookup for Numbers mask type. |
| Val8 | `9` | Indicates Lookup for Flags mask type. |
| Val9 | `10` | Indicates Lookup for FinishDate mask type. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


