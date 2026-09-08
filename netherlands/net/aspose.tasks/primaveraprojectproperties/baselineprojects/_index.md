---
title: "PrimaveraProjectProperties.BaselineProjects"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PrimaveraProjectProperties eigenschap. Haalt een array op van baselineprojecten van het huidige project. Is toepasbaar op projecten die zijn gelezen uit Primavera XML-bestanden met geëxporteerde baselines"
type: docs
weight: 10
url: /nl/net/aspose.tasks/primaveraprojectproperties/baselineprojects/
---
## PrimaveraProjectProperties.BaselineProjects property

Haalt een array op van baselineprojecten van het huidige project. Is van toepassing op projecten die zijn gelezen uit Primavera XML-bestanden met geëxporteerde baselines.

```csharp
public Project[] BaselineProjects { get; }
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

* class [Project](../../project/)
* class [PrimaveraProjectProperties](../)
* namespace [Aspose.Tasks](../../primaveraprojectproperties/)
* assembly [Aspose.Tasks](../../../)


