---
title: PrimaveraProjectProperties.BaselineProjects
second_title: Aspose.Tasks for .NET API Reference
description: PrimaveraProjectProperties property. Gets array of baseline projects of current project. Is applicable to projects read from Primavera XML files containing exported baselines
type: docs
weight: 10
url: /net/aspose.tasks/primaveraprojectproperties/baselineprojects/
---
## PrimaveraProjectProperties.BaselineProjects property

Gets array of baseline projects of current project. Is applicable to projects read from Primavera XML files containing exported baselines.

```csharp
public Project[] BaselineProjects { get; }
```

## Examples

Shows how to read a project from a Primavera XML file and examine baseline project data.

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

### See Also

* class [Project](../../project/)
* class [PrimaveraProjectProperties](../)
* namespace [Aspose.Tasks](../../primaveraprojectproperties/)
* assembly [Aspose.Tasks](../../../)


