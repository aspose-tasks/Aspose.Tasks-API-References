---
title: "PrimaveraProjectProperties.CurrentBaselineProjectId"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PrimaveraProjectProperties eigenschap. Haalt de ID op van het huidige baselineproject. Is van toepassing op projecten die worden gelezen uit Primavera XML-bestanden met geëxporteerde baselines"
type: docs
weight: 40
url: /nl/net/aspose.tasks/primaveraprojectproperties/currentbaselineprojectid/
---
## PrimaveraProjectProperties.CurrentBaselineProjectId property

Haalt de Id op van het huidige baselineproject. Is van toepassing op projecten die zijn gelezen uit Primavera XML-bestanden met geëxporteerde baselines.

```csharp
public int CurrentBaselineProjectId { get; }
```

## Voorbeelden

Toont hoe een project te lezen uit een Primavera XML-bestand en baselineprojectgegevens te onderzoeken.

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

### Zie ook

* class [PrimaveraProjectProperties](../)
* namespace [Aspose.Tasks](../../primaveraprojectproperties/)
* assembly [Aspose.Tasks](../../../)


