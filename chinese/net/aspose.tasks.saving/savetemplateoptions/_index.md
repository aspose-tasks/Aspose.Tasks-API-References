---
title: "类 SaveTemplateOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Saving.SaveTemplateOptions 类。允许在将项目保存为模板时指定其他选项"
type: docs
weight: 2200
url: /zh/net/aspose.tasks.saving/savetemplateoptions/
---
## SaveTemplateOptions class

允许在将项目保存为模板时指定附加选项。

```csharp
public class SaveTemplateOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [SaveTemplateOptions](savetemplateoptions/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [RemoveActualValues](../../aspose.tasks.saving/savetemplateoptions/removeactualvalues/) { get; set; } | 获取或设置一个值，指示是否应删除项目模板中的所有实际值。 |
| [RemoveBaselineValues](../../aspose.tasks.saving/savetemplateoptions/removebaselinevalues/) { get; set; } | 获取或设置一个值，指示是否应删除项目模板中的所有基线值。 |
| [RemoveFixedCosts](../../aspose.tasks.saving/savetemplateoptions/removefixedcosts/) { get; set; } | 获取或设置一个值，指示是否应删除项目模板中的所有固定成本。 |
| [RemoveResourceRates](../../aspose.tasks.saving/savetemplateoptions/removeresourcerates/) { get; set; } | 获取或设置一个值，指示是否应删除项目模板中的资源费率。 |

## 示例

展示如何使用选项将项目保存为模板。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
var projectFileInfo = Project.GetProjectFileInfo(DataDir + "EstimatedMilestoneTasks.mpp");

Console.WriteLine("Project File Format: " + projectFileInfo.ProjectFileFormat);

// 创建模板保存选项
// 并调整其属性
var options = new SaveTemplateOptions
{
    // 设置一个值，指示是否应删除项目模板中的所有固定成本
    RemoveFixedCosts = true,

    // 设置一个值，指示是否应删除项目模板中的所有实际值
    RemoveActualValues = true,

    // 设置一个值，指示是否应删除项目模板中的资源费率
    RemoveResourceRates = true,

    // 设置一个值，指示是否应删除项目模板中的所有基线值
    RemoveBaselineValues = true
};

project.SaveAsTemplate(OutDir + "SaveProjectDataAsTemplate_out.mpt", options);

var templateFileInfo = Project.GetProjectFileInfo(DataDir + "SaveProjectDataAsTemplate_out.mpt");
Console.WriteLine("Project File Format: " + templateFileInfo.ProjectFileFormat);
```

### 另见

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


