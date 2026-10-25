---
title: "类 WBSCodeMask"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.WBSCodeMask 类。表示 WBS 代码掩码"
type: docs
weight: 3500
url: /zh/net/aspose.tasks/wbscodemask/
---
## WBSCodeMask class

表示 WBS 代码掩码。

```csharp
public class WBSCodeMask
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [WBSCodeMask](wbscodemask/)() | 初始化 `WBSCodeMask` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Length](../../aspose.tasks/wbscodemask/length/) { get; set; } | 获取或设置代码字符串的字符数。 |
| [Level](../../aspose.tasks/wbscodemask/level/) { get; } | 获取掩码级别。 |
| [Separator](../../aspose.tasks/wbscodemask/separator/) { get; set; } | 获取或设置代码字符串的分隔符。默认值为句点。 |
| [Sequence](../../aspose.tasks/wbscodemask/sequence/) { get; set; } | 获取或设置代码字符串的字符类型。 |

## 示例

展示如何创建 WBS 代码掩码。

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

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


