---
title: OutlineMask.Length
second_title: Aspose.Tasks for .NET API Reference
description: OutlineMask property. Gets or sets the maximum length in characters of the outline code values. 0 if length is not defined
type: docs
weight: 20
url: /net/aspose.tasks/outlinemask/length/
---
## OutlineMask.Length property

Gets or sets the maximum length (in characters) of the outline code values. 0 if length is not defined.

```csharp
public int Length { get; set; }
```

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

* class [OutlineMask](../)
* namespace [Aspose.Tasks](../../outlinemask/)
* assembly [Aspose.Tasks](../../../)


