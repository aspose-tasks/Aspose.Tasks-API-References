---
title: Enum WBSSequence
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.WBSSequence enum. Specifies sequence for WBSCodeMask
type: docs
weight: 3500
url: /net/aspose.tasks/wbssequence/
---
## WBSSequence enumeration

Specifies sequence for WBSCodeMask

```csharp
public enum WBSSequence
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| OrderedNumbers | `0` | Indicates Numbers WBS sequence. |
| OrderedUppercaseLetters | `1` | Indicates Uppercase letters WBS sequence. |
| OrderedLowercaseLetters | `2` | Indicates Lowercase letters WBS sequence. |
| UnorderedCharacters | `3` | Indicates Unordered characters WBS sequence. |

## Examples

Shows how to set WBS sequences.

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


