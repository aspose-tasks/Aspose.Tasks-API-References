---
title: "Task.Assignments"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà di Task. Ottiene una raccolta di assegnazioni di risorse per questo oggetto"
type: docs
weight: 120
url: /it/net/aspose.tasks/task/assignments/
---
## Task.Assignments property

Ottiene una raccolta di assegnazioni di risorse per questo oggetto.

```csharp
public ResourceAssignmentCollection Assignments { get; }
```

## Esempi

Mostra come iterare le assegnazioni dell'attività.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // visualizza le assegnazioni del task
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### Vedi anche

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


