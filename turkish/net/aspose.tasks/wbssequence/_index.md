---
title: "Enum WBSSequence"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.WBSSequence enum. WBSCodeMask için sıralamayı belirtir."
type: docs
weight: 3520
url: /tr/net/aspose.tasks/wbssequence/
---
## WBSSequence enumeration

WBSCodeMask için sıralamayı belirtir.

```csharp
public enum WBSSequence
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| OrderedNumbers | `0` | Sayılar WBS sıralamasını gösterir. |
| OrderedUppercaseLetters | `1` | Büyük harfler WBS sıralamasını gösterir. |
| OrderedLowercaseLetters | `2` | Küçük harfler WBS sıralamasını gösterir. |
| UnorderedCharacters | `3` | Sırasız karakterler WBS sıralamasını gösterir. |

## Örnekler

WBS sıralamalarının nasıl ayarlanacağını gösterir.

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

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


