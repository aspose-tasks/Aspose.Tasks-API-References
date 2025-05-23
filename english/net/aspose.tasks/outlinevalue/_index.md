---
title: Class OutlineValue
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.OutlineValue class. Represents an outline value
type: docs
weight: 1200
url: /net/aspose.tasks/outlinevalue/
---
## OutlineValue class

Represents an outline value.

```csharp
public class OutlineValue
```

## Constructors

| Name | Description |
| --- | --- |
| [OutlineValue](outlinevalue/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [Description](../../aspose.tasks/outlinevalue/description/) { get; set; } | Gets or sets the description of an outline value. |
| [DurationValue](../../aspose.tasks/outlinevalue/durationvalue/) { get; set; } | Gets or sets the duration if Type is Duration. |
| [IsCollapsed](../../aspose.tasks/outlinevalue/iscollapsed/) { get; set; } | Gets or sets a value indicating whether outline value is collapsed or not. |
| [ParentValueId](../../aspose.tasks/outlinevalue/parentvalueid/) { get; set; } | Gets or sets the Id of a parent node of an outline code. |
| [Type](../../aspose.tasks/outlinevalue/type/) { get; set; } | Gets or sets the outline code type. |
| [Value](../../aspose.tasks/outlinevalue/value/) { get; set; } | Gets or sets the actual value. |
| [ValueGuid](../../aspose.tasks/outlinevalue/valueguid/) { get; } | Gets a GUID which identifies this value among others in the entire project. |
| [ValueId](../../aspose.tasks/outlinevalue/valueid/) { get; set; } | Gets or sets the unique Id of an outline code value within a project. |

## Examples

Shows how to work with outline values.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = new OutlineCodeDefinition();
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline.Alias = "My Outline Code";
var outline2 = new OutlineCodeDefinition();
outline2.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline2.Alias = "My Outline Code 2";

project.OutlineCodes.Add(outline);

var mask = new OutlineMask();
mask.Type = MaskType.Characters;
outline.Masks.Add(mask);

// create an outline value
var value = new OutlineValue();

// set the actual value
value.Value = "Text value 1";

// set the unique Id of an outline code value within a project
value.ValueId = 1;

// get a GUID which identifies this value among others in the entire project
Console.WriteLine("Check value GUID: " + value.ValueGuid);

// set the outline code type
value.Type = OutlineValueType.Text;

// set the description of an outline value
value.Description = "Text value descr 1";

// set a value indicating whether outline value is collapsed or not
value.IsCollapsed = false;

// check parent value id
Console.WriteLine("Check parent value id: " + value.ParentValueId);
outline.Values.Add(value);

// create an outline value with duration
var value2 = new OutlineValue();

// set the duration value
value2.DurationValue = project.GetDuration(1, TimeUnitType.Hour);

// set the unique Id of an outline code value within a project
value2.ValueId = 2;
outline2.Values.Add(value2);

// ...
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


