---
title: "枚举 WBSSequence"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.WBSSequence 枚举。指定 WBSCodeMask 的序列"
type: docs
weight: 3520
url: /zh/net/aspose.tasks/wbssequence/
---
## WBSSequence enumeration

指定 WBSCodeMask 的顺序

```csharp
public enum WBSSequence
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| OrderedNumbers | `0` | 指示数字 WBS 序列。 |
| OrderedUppercaseLetters | `1` | 指示大写字母 WBS 序列。 |
| OrderedLowercaseLetters | `2` | 指示小写字母 WBS 序列。 |
| UnorderedCharacters | `3` | 指示无序字符 WBS 序列。 |

## 示例

展示如何设置 WBS 序列。

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

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


