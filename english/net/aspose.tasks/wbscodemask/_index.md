---
title: Class WBSCodeMask
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.WBSCodeMask class. Represents WBS Code mask
type: docs
weight: 3480
url: /net/aspose.tasks/wbscodemask/
---
## WBSCodeMask class

Represents WBS Code mask.

```csharp
public class WBSCodeMask
```

## Constructors

| Name | Description |
| --- | --- |
| [WBSCodeMask](wbscodemask/)() | Initializes a new instance of the `WBSCodeMask` class. |

## Properties

| Name | Description |
| --- | --- |
| [Length](../../aspose.tasks/wbscodemask/length/) { get; set; } | Gets or sets the number of characters of the code string. |
| [Level](../../aspose.tasks/wbscodemask/level/) { get; } | Gets the mask level. |
| [Separator](../../aspose.tasks/wbscodemask/separator/) { get; set; } | Gets or sets the separator of the code string. Default value is Period. |
| [Sequence](../../aspose.tasks/wbscodemask/sequence/) { get; set; } | Gets or sets the type of character of the code string. |

## Examples

Shows how to create WBS code masks.

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

var task = project.RootTask.Children.Add("Task 1");
task.Children.Add("Task 2");

project.Recalculate();

Console.WriteLine("Number of WBS masks: " + project.WBSCodeDefinition.CodeMaskCollection.Count);
var i = 0;
foreach (var cm in project.WBSCodeDefinition.CodeMaskCollection)
{
    Console.WriteLine("WBS Mask #{0}: Level->{1}", ++i, cm.Level);
}

project.Save(OutDir + @"AddWBSCodes_out.xml", SaveFileFormat.Xml);
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


