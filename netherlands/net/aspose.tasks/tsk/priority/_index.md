---
title: "Tsk.Priority"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. Het belangsniveau dat aan een taak wordt toegekend, wat op zijn beurt aangeeft hoe gemakkelijk een taak of toewijzing kan worden uitgesteld of gesplitst tijdens resource-leveling."
type: docs
weight: 930
url: /nl/net/aspose.tasks/tsk/priority/
---
## Tsk.Priority field

Het belangsniveau dat aan een taak wordt toegekend, wat op zijn beurt aangeeft hoe gemakkelijk een taak of toewijzing kan worden vertraagd of gesplitst tijdens resource-leveling.

```csharp
public static readonly Key<int, TaskKey> Priority;
```

## Voorbeelden

Toont hoe een taakprioriteit te lezen.

```csharp
var project = new Project(DataDir + "TaskPriority.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Toon prioriteiten voor alle taken
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name) + " - Priority : " + task.Get(Tsk.Priority));
}
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


