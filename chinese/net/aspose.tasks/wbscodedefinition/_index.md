---
title: "类 WBSCodeDefinition"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.WBSCodeDefinition 类。表示一个 WBS 代码定义。"
type: docs
weight: 3490
url: /zh/net/aspose.tasks/wbscodedefinition/
---
## WBSCodeDefinition class

表示 WBS 代码定义。

```csharp
public class WBSCodeDefinition
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [WBSCodeDefinition](wbscodedefinition/)() | 初始化 `WBSCodeDefinition` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [CodeMaskCollection](../../aspose.tasks/wbscodedefinition/codemaskcollection/) { get; } | 获取 WBSCodeMask 对象的集合。 |
| [CodePrefix](../../aspose.tasks/wbscodedefinition/codeprefix/) { get; set; } | 获取或设置项目代码前缀。 |
| [GenerateWBSCode](../../aspose.tasks/wbscodedefinition/generatewbscode/) { get; set; } | 获取或设置一个值，指示是否为新任务生成 WBS 代码。 |
| [VerifyUniqueness](../../aspose.tasks/wbscodedefinition/verifyuniqueness/) { get; set; } | 获取或设置一个值，指示是否验证新 WBS 代码的唯一性。 |

## 示例

展示如何添加 WBS 代码掩码。

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


