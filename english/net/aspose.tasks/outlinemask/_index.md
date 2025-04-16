---
title: Class OutlineMask
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.OutlineMask class. Represents four elements of a mask which defines an outline code format
type: docs
weight: 1180
url: /net/aspose.tasks/outlinemask/
---
## OutlineMask class

Represents four elements of a mask which defines an outline code format.

```csharp
public class OutlineMask
```

## Constructors

| Name | Description |
| --- | --- |
| [OutlineMask](outlinemask/)() | Initializes a new instance of the `OutlineMask` class. |

## Properties

| Name | Description |
| --- | --- |
| [Length](../../aspose.tasks/outlinemask/length/) { get; set; } | Gets or sets the maximum length (in characters) of the outline code values. 0 if length is not defined. |
| [Level](../../aspose.tasks/outlinemask/level/) { get; set; } | Gets or sets the level of a mask. |
| [Separator](../../aspose.tasks/outlinemask/separator/) { get; set; } | Gets or sets the separator of code values. |
| [Type](../../aspose.tasks/outlinemask/type/) { get; set; } | Gets or sets the type of a mask. |

## Examples

Shows how to work with outline masks.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = new OutlineCodeDefinition();
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline.Alias = "My Outline Code";

project.OutlineCodes.Add(outline);

var mask = new OutlineMask();

// set the type of a mask
mask.Type = MaskType.Characters;

// set the separator of code values
mask.Separator = "/";

// set the level of a mask
mask.Level = 1;

// set the maximum length (in characters) of the outline code values. 0 if length is not defined.
mask.Length = 2;

// add the mask to the definition
outline.Masks.Add(mask);

var value = new OutlineValue();
value.Value = "Text value 1";
value.ValueId = 1;
value.Type = OutlineValueType.Text;
value.Description = "Text value descr 1";
outline.Values.Add(value);

// ...
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


