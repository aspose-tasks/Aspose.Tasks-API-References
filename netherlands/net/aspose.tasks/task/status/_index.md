---
title: "Task.Status"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Taakeigenschap. Haalt de status van de taak op."
type: docs
weight: 1160
url: /nl/net/aspose.tasks/task/status/
---
## Task.Status property

Haalt de taakstatus op.

```csharp
public TaskStatus Status { get; }
```

## Voorbeelden

Toont hoe u de status van de taak kunt ophalen.

```csharp
var project = new Project(DataDir + "TaskPercentageCompletion.mpp");

// De statusdatum van het project moet worden ingesteld omdat de statusberekening de statusdatum gebruikt.
project.StatusDate = new DateTime(2010, 7, 9, 15, 0, 0);
foreach (var task in project.EnumerateAllChildTasks())
{
    Console.WriteLine("{0} - {1}", task.Name, task.Status);
}
```

### Zie ook

* enum [TaskStatus](../../taskstatus/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


