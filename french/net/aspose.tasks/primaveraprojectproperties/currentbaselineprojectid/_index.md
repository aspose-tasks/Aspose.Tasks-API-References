---
title: "PrimaveraProjectProperties.CurrentBaselineProjectId"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété PrimaveraProjectProperties. Obtient l'ID du projet de référence actuel. S'applique aux projets lus à partir de fichiers XML Primavera contenant des références exportées"
type: docs
weight: 40
url: /fr/net/aspose.tasks/primaveraprojectproperties/currentbaselineprojectid/
---
## PrimaveraProjectProperties.CurrentBaselineProjectId property

Obtient l'Id du projet de référence actuel. S'applique aux projets lus à partir de fichiers XML Primavera contenant des références exportées.

```csharp
public int CurrentBaselineProjectId { get; }
```

## Exemples

Montre comment lire un projet à partir d'un fichier XML Primavera et examiner les données du projet de référence.

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

### Voir aussi

* class [PrimaveraProjectProperties](../)
* namespace [Aspose.Tasks](../../primaveraprojectproperties/)
* assembly [Aspose.Tasks](../../../)


