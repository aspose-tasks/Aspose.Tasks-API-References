---
title: "Task.Assignments"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Task eigenschap. Haalt een verzameling van resource-toewijzingen op voor dit object"
type: docs
weight: 120
url: /nl/net/aspose.tasks/task/assignments/
---
## Task.Assignments property

Haalt een verzameling van resource-toewijzingen op voor dit object.

```csharp
public ResourceAssignmentCollection Assignments { get; }
```

## Voorbeelden

Toont hoe je over de toewijzingen van een taak kunt itereren.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // toon de toewijzingen van de taak
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### Zie ook

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


