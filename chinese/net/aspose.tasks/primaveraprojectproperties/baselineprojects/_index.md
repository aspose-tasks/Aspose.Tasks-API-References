---
title: "PrimaveraProjectProperties.BaselineProjects"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PrimaveraProjectProperties 属性。获取当前项目的基线项目数组。适用于从包含已导出基线的 Primavera XML 文件读取的项目"
type: docs
weight: 10
url: /zh/net/aspose.tasks/primaveraprojectproperties/baselineprojects/
---
## PrimaveraProjectProperties.BaselineProjects property

获取当前项目的基线项目数组。适用于从包含已导出基线的 Primavera XML 文件读取的项目。

```csharp
public Project[] BaselineProjects { get; }
```

## 示例

展示如何从 Primavera XML 文件读取项目并检查基线项目数据。

```csharp
Project project = new Project(DataDir + "BaselineProjects.xml");

Console.WriteLine("Current baseline project uid: " + project.PrimaveraProperties.CurrentBaselineProjectId);

foreach (var baselineProject in project.PrimaveraProperties.BaselineProjects)
{
    Console.WriteLine("Baseline project: uid: {0}, name: '{1}'", baselineProject.Uid, baselineProject.Name);
}

var baseline1 = project.PrimaveraProperties.BaselineProjects[1];

var task = GetTaskByActivityId(project, "A1000");
var baselineTask = GetTaskByActivityId(baseline1, "A1000");

Console.WriteLine("Task budgeted total cost: " + task.PrimaveraProperties.BudgetedTotalCost);
Console.WriteLine("Task baseline budgeted total cost: " + baselineTask.PrimaveraProperties.BudgetedTotalCost);
```

### 另见

* class [Project](../../project/)
* class [PrimaveraProjectProperties](../)
* namespace [Aspose.Tasks](../../primaveraprojectproperties/)
* assembly [Aspose.Tasks](../../../)


