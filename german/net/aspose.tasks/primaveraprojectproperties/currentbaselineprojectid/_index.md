---
title: "PrimaveraProjectProperties.CurrentBaselineProjectId"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "PrimaveraProjectProperties-Eigenschaft. Gibt die ID des aktuellen Basislinienprojekts zurück. Ist anwendbar auf Projekte, die aus Primavera-XML-Dateien mit exportierten Basislinien gelesen werden."
type: docs
weight: 40
url: /de/net/aspose.tasks/primaveraprojectproperties/currentbaselineprojectid/
---
## PrimaveraProjectProperties.CurrentBaselineProjectId property

Liefert die ID des aktuellen Basislinienprojekts. Ist anwendbar auf Projekte, die aus Primavera-XML-Dateien mit exportierten Basislinien gelesen werden.

```csharp
public int CurrentBaselineProjectId { get; }
```

## Beispiele

Zeigt, wie ein Projekt aus einer Primavera-XML-Datei gelesen und Basisliniendaten des Projekts untersucht werden.

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

### Siehe auch

* class [PrimaveraProjectProperties](../)
* namespace [Aspose.Tasks](../../primaveraprojectproperties/)
* assembly [Aspose.Tasks](../../../)


