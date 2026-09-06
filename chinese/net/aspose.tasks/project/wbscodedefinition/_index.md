---
title: "Project.WBSCodeDefinition"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 属性。获取或设置项目的 WBS Code Definition"
type: docs
weight: 1030
url: /zh/net/aspose.tasks/project/wbscodedefinition/
---
## Project.WBSCodeDefinition property

获取或设置项目的 WBS 代码定义。

```csharp
public WBSCodeDefinition WBSCodeDefinition { get; set; }
```

## 示例

展示如何添加 WBS 代码。

```csharp
var project = new Project
{
    WBSCodeDefinition = new WBSCodeDefinition()
};
project.WBSCodeDefinition.GenerateWBSCode = true;
project.WBSCodeDefinition.VerifyUniqueness = true;
project.WBSCodeDefinition.CodePrefix = "CRS-";

var mask = new WBSCodeMask
{
    Length = 2,
    Separator = "-",
    Sequence = WBSSequence.OrderedNumbers
};
project.WBSCodeDefinition.CodeMaskCollection.Add(mask);

mask = new WBSCodeMask
{
    Length = 1,
    Separator = "-",
    Sequence = WBSSequence.OrderedUppercaseLetters
};
project.WBSCodeDefinition.CodeMaskCollection.Add(mask);

var tsk = project.RootTask.Children.Add("Task 1");
tsk.Children.Add("Task 2");

project.Recalculate();

project.Save(OutDir + @"AddWBSCodes_out.xml", SaveFileFormat.Xml);
```

### 另见

* class [WBSCodeDefinition](../../wbscodedefinition/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


