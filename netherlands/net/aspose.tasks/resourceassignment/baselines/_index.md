---
title: "ResourceAssignment.Baselines"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ResourceAssignment property. Haalt AssignmentBaselineCollection-object op. De verzameling van baseline-waarden die aan een toewijzing zijn gekoppeld"
type: docs
weight: 120
url: /nl/net/aspose.tasks/resourceassignment/baselines/
---
## ResourceAssignment.Baselines property

Haalt AssignmentBaselineCollection‑object op. De verzameling van baseline‑waarden die aan een toewijzing zijn gekoppeld.

```csharp
public AssignmentBaselineCollection Baselines { get; }
```

## Voorbeelden

Toont hoe toegang te krijgen tot de baselines van een toewijzing.

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

### Zie ook

* class [AssignmentBaselineCollection](../../assignmentbaselinecollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


