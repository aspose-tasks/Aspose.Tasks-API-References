---
title: "Tsk.OutlineLevel"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. Het outline‑niveau van een taak."
type: docs
weight: 840
url: /nl/net/aspose.tasks/tsk/outlinelevel/
---
## Tsk.OutlineLevel field

Het outline-niveau van een taak.

```csharp
public static readonly Key<int, TaskKey> OutlineLevel;
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


