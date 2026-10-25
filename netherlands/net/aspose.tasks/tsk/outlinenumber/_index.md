---
title: "Tsk.OutlineNumber"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Het nummer dat de positie van een taak in de hiërarchische outline-structuur weergeeft."
type: docs
weight: 850
url: /nl/net/aspose.tasks/tsk/outlinenumber/
---
## Tsk.OutlineNumber field

Het nummer dat de positie van een taak in de hiërarchische outline-structuur aangeeft.

```csharp
public static readonly Key<string, TaskKey> OutlineNumber;
```

## Voorbeelden

Toont hoe de outline‑eigenschappen van een taak te lezen.

```csharp
var project = new Project(DataDir + "TaskOutlineProperties.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Alle verzamelde taken doorlopen
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name) + " - Outline Level : " + task.Get(Tsk.OutlineLevel));
    Console.WriteLine(task.Get(Tsk.Name) + " - Outline Number : " + task.Get(Tsk.OutlineNumber));
}
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


