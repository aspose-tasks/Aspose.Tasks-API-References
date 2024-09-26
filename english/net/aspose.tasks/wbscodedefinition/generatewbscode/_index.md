---
title: WBSCodeDefinition.GenerateWBSCode
second_title: Aspose.Tasks for .NET API Reference
description: WBSCodeDefinition property. Gets or sets a value indicating whether to generate WBS code for new task
type: docs
weight: 40
url: /net/aspose.tasks/wbscodedefinition/generatewbscode/
---
## WBSCodeDefinition.GenerateWBSCode property

Gets or sets a value indicating whether to generate WBS code for new task.

```csharp
public bool GenerateWBSCode { get; set; }
```

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

* class [WBSCodeDefinition](../)
* namespace [Aspose.Tasks](../../wbscodedefinition/)
* assembly [Aspose.Tasks](../../../)


