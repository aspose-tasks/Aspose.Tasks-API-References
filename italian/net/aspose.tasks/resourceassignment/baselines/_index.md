---
title: "ResourceAssignment.Baselines"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ResourceAssignment. Ottiene l'oggetto AssignmentBaselineCollection. La raccolta dei valori di baseline associati a un'assegnazione"
type: docs
weight: 120
url: /it/net/aspose.tasks/resourceassignment/baselines/
---
## ResourceAssignment.Baselines property

Ottiene l'oggetto AssignmentBaselineCollection. La collezione di valori di baseline associati a un'assegnazione.

```csharp
public AssignmentBaselineCollection Baselines { get; }
```

## Esempi

Mostra come accedere alle baseline dell'assegnazione.

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

### Vedi anche

* class [AssignmentBaselineCollection](../../assignmentbaselinecollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


