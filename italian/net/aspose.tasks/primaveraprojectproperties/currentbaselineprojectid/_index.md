---
title: "PrimaveraProjectProperties.CurrentBaselineProjectId"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà PrimaveraProjectProperties. Ottiene l'Id del progetto baseline corrente. È applicabile ai progetti letti da file XML Primavera contenenti baseline esportate"
type: docs
weight: 40
url: /it/net/aspose.tasks/primaveraprojectproperties/currentbaselineprojectid/
---
## PrimaveraProjectProperties.CurrentBaselineProjectId property

Ottiene l'Id del progetto di baseline corrente. È applicabile ai progetti letti da file XML di Primavera contenenti baseline esportate.

```csharp
public int CurrentBaselineProjectId { get; }
```

## Esempi

Mostra come leggere un progetto da un file XML di Primavera ed esaminare i dati del progetto di baseline.

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

### Vedi anche

* class [PrimaveraProjectProperties](../)
* namespace [Aspose.Tasks](../../primaveraprojectproperties/)
* assembly [Aspose.Tasks](../../../)


