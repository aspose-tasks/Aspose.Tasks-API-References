---
title: "SaveTemplateOptions.RemoveBaselineValues"
second_title: "Aspose.Tasks for .NET API 参考"
description: "SaveTemplateOptions 属性。获取或设置一个值，指示是否应从项目模板中删除所有基线值"
type: docs
weight: 30
url: /zh/net/aspose.tasks.saving/savetemplateoptions/removebaselinevalues/
---
## SaveTemplateOptions.RemoveBaselineValues property

获取或设置一个值，指示是否应删除项目模板中的所有基线值。

```csharp
public bool RemoveBaselineValues { get; set; }
```

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

* class [SaveTemplateOptions](../)
* namespace [Aspose.Tasks.Saving](../../savetemplateoptions/)
* assembly [Aspose.Tasks](../../../)


