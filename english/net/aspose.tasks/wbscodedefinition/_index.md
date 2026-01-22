---
title: Class WBSCodeDefinition
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.WBSCodeDefinition class. Represents a WBS Code Definition
type: docs
weight: 3460
url: /net/aspose.tasks/wbscodedefinition/
---
## WBSCodeDefinition class

Represents a WBS Code Definition.

```csharp
public class WBSCodeDefinition
```

## Constructors

| Name | Description |
| --- | --- |
| [WBSCodeDefinition](wbscodedefinition/)() | Initializes a new instance of the `WBSCodeDefinition` class. |

## Properties

| Name | Description |
| --- | --- |
| [CodeMaskCollection](../../aspose.tasks/wbscodedefinition/codemaskcollection/) { get; } | Gets the collection of WBSCodeMask objects. |
| [CodePrefix](../../aspose.tasks/wbscodedefinition/codeprefix/) { get; set; } | Gets or sets the project code prefix. |
| [GenerateWBSCode](../../aspose.tasks/wbscodedefinition/generatewbscode/) { get; set; } | Gets or sets a value indicating whether to generate WBS code for new task. |
| [VerifyUniqueness](../../aspose.tasks/wbscodedefinition/verifyuniqueness/) { get; set; } | Gets or sets a value indicating whether to verify uniqueness of new WBS codes. |

## Examples

Shows how to add WBS code masks.

```csharp
var project = new Project();

project.WBSCodeDefinition = new WBSCodeDefinition();
project.WBSCodeDefinition.GenerateWBSCode = true;
project.WBSCodeDefinition.VerifyUniqueness = true;
project.WBSCodeDefinition.CodePrefix = "CRS-";

var mask = new WBSCodeMask();
mask.Length = 2;
mask.Separator = "-";
mask.Sequence = WBSSequence.OrderedNumbers;
project.WBSCodeDefinition.CodeMaskCollection.Add(mask);

mask = new WBSCodeMask();
mask.Length = 1;
mask.Separator = "-";
mask.Sequence = WBSSequence.OrderedUppercaseLetters;
project.WBSCodeDefinition.CodeMaskCollection.Add(mask);

var tsk = project.RootTask.Children.Add("Task 1");
tsk.Children.Add("Task 2");

project.Recalculate();

project.Save(OutDir + @"AddWBSCodes_out.xml", SaveFileFormat.Xml);
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


