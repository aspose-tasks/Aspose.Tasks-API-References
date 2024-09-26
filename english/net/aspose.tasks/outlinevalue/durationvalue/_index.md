---
title: OutlineValue.DurationValue
second_title: Aspose.Tasks for .NET API Reference
description: OutlineValue property. Gets or sets the duration if Type is Duration
type: docs
weight: 30
url: /net/aspose.tasks/outlinevalue/durationvalue/
---
## OutlineValue.DurationValue property

Gets or sets the duration if Type is Duration.

```csharp
public Duration? DurationValue { get; set; }
```

## Remarks

Prefer this property over the [`Value`](../value/), when you need to set the value for OutlineValues with Duration type .

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

* struct [Duration](../../duration/)
* class [OutlineValue](../)
* namespace [Aspose.Tasks](../../outlinevalue/)
* assembly [Aspose.Tasks](../../../)


