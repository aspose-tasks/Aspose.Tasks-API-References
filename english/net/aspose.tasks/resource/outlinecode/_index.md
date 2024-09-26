---
title: Resource.OutlineCode
second_title: Aspose.Tasks for .NET API Reference
description: Resource property. Gets an OutlineCodeCollection object. The value of an outline code
type: docs
weight: 540
url: /net/aspose.tasks/resource/outlinecode/
---
## Resource.OutlineCode property

Gets an OutlineCodeCollection object. The value of an outline code.

```csharp
public OutlineCodeCollection OutlineCode { get; }
```

## Remarks

Two pieces of data are necessary - a pointer to the outline code table that is specified by the FieldID, and the value that is specified either by the ValueID or ValueGUID pointer to the value list.

## Examples

Shows how to work with resource outline values.

```csharp
var project = new Project(DataDir + "OutlineCodes2003.mpp");

var res = project.Resources.GetById(2);
Assert.AreEqual(2, res.OutlineCode.Count);
foreach (var code in res.OutlineCode)
{
    object val = null;
    foreach (var def in project.OutlineCodes)
    {
        if (def.FieldId != code.FieldId)
        {
            continue;
        }

        foreach (var value in def.Values)
        {
            if (value.ValueId != code.ValueId)
            {
                continue;
            }

            val = value.Value;
            break;
        }
    }

    Console.WriteLine(val.ToString());
}
```

### See Also

* class [OutlineCodeCollection](../../outlinecodecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


