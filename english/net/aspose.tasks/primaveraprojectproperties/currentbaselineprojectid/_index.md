---
title: PrimaveraProjectProperties.CurrentBaselineProjectId
second_title: Aspose.Tasks for .NET API Reference
description: PrimaveraProjectProperties property. Gets Id of the current baseline project. Is applicable to projects read from Primavera XML files containing exported baselines
type: docs
weight: 20
url: /net/aspose.tasks/primaveraprojectproperties/currentbaselineprojectid/
---
## PrimaveraProjectProperties.CurrentBaselineProjectId property

Gets Id of the current baseline project. Is applicable to projects read from Primavera XML files containing exported baselines.

```csharp
public int CurrentBaselineProjectId { get; }
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

* class [PrimaveraProjectProperties](../)
* namespace [Aspose.Tasks](../../primaveraprojectproperties/)
* assembly [Aspose.Tasks](../../../)


