---
title: "ResourceAssignment.Baselines"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "ResourceAssignment property. Obtient l'objet AssignmentBaselineCollection. La collection des valeurs de repère associées à une affectation"
type: docs
weight: 120
url: /fr/net/aspose.tasks/resourceassignment/baselines/
---
## ResourceAssignment.Baselines property

Obtient l'objet AssignmentBaselineCollection. La collection des valeurs de base associées à une affectation.

```csharp
public AssignmentBaselineCollection Baselines { get; }
```

## Exemples

Montre comment accéder aux repères d'une affectation.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

project.SetBaseline(BaselineType.Baseline);

foreach (var assignmentBaseline in resourceAssignment.Baselines)
{
    Console.WriteLine("Baseline Start: {0}", assignmentBaseline.Start);
    Console.WriteLine("Baseline Finish: {0}", assignmentBaseline.Finish);
}
```

### Voir aussi

* class [AssignmentBaselineCollection](../../assignmentbaselinecollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


