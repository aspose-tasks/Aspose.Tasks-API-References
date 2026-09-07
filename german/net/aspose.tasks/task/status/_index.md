---
title: "Task.Status"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "Task‑Eigenschaft. Gibt den Task‑Status zurück"
type: docs
weight: 1160
url: /de/net/aspose.tasks/task/status/
---
## Task.Status property

Gibt den Task‑Status zurück.

```csharp
public TaskStatus Status { get; }
```

## Beispiele

Zeigt, wie der Task‑Status abgerufen wird.

```csharp
var project = new Project(DataDir + "TaskPercentageCompletion.mpp");

// Das Statusdatum des Projekts sollte festgelegt werden, da die Statusberechnung das Statusdatum verwendet.
project.StatusDate = new DateTime(2010, 7, 9, 15, 0, 0);
foreach (var task in project.EnumerateAllChildTasks())
{
    Console.WriteLine("{0} - {1}", task.Name, task.Status);
}
```

### Siehe auch

* enum [TaskStatus](../../taskstatus/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


