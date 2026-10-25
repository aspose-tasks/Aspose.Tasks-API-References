---
title: "PrimaveraProjectProperties.BaselineProjects"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "PrimaveraProjectProperties propriété. Obtient un tableau de projets de référence du projet actuel. S'applique aux projets lus à partir de fichiers XML Primavera contenant des bases de référence exportées"
type: docs
weight: 10
url: /fr/net/aspose.tasks/primaveraprojectproperties/baselineprojects/
---
## PrimaveraProjectProperties.BaselineProjects property

Obtient le tableau des projets de référence du projet actuel. S'applique aux projets lus à partir de fichiers XML Primavera contenant des références exportées.

```csharp
public Project[] BaselineProjects { get; }
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

* class [Project](../../project/)
* class [PrimaveraProjectProperties](../)
* namespace [Aspose.Tasks](../../primaveraprojectproperties/)
* assembly [Aspose.Tasks](../../../)


