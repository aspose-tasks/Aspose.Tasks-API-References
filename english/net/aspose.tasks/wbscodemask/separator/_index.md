---
title: WBSCodeMask.Separator
second_title: Aspose.Tasks for .NET API Reference
description: WBSCodeMask property. Gets or sets the separator of the code string. Default value is Period
type: docs
weight: 40
url: /net/aspose.tasks/wbscodemask/separator/
---
## WBSCodeMask.Separator property

Gets or sets the separator of the code string. Default value is Period.

```csharp
public string Separator { get; set; }
```

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

* class [WBSCodeMask](../)
* namespace [Aspose.Tasks](../../wbscodemask/)
* assembly [Aspose.Tasks](../../../)


