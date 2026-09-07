---
title: "PrimaveraProjectProperties.BaselineProjects"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "PrimaveraProjectProperties-Eigenschaft. Gibt ein Array von Basislinienprojekten des aktuellen Projekts zurück. Ist anwendbar auf Projekte, die aus Primavera-XML-Dateien mit exportierten Basislinien gelesen werden."
type: docs
weight: 10
url: /de/net/aspose.tasks/primaveraprojectproperties/baselineprojects/
---
## PrimaveraProjectProperties.BaselineProjects property

Ruft ein Array von Basislinienprojekten des aktuellen Projekts ab. Gilt für Projekte, die aus Primavera‑XML‑Dateien mit exportierten Basislinien gelesen wurden.

```csharp
public Project[] BaselineProjects { get; }
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

* class [Project](../../project/)
* class [PrimaveraProjectProperties](../)
* namespace [Aspose.Tasks](../../primaveraprojectproperties/)
* assembly [Aspose.Tasks](../../../)


