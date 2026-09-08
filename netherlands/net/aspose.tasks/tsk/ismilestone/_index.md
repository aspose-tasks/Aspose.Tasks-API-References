---
title: "Tsk.IsMilestone"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Bepaalt of een taak een mijlpaal is."
type: docs
weight: 630
url: /nl/net/aspose.tasks/tsk/ismilestone/
---
## Tsk.IsMilestone field

Bepaalt of een taak een mijlpaal is.

```csharp
public static readonly Key<NullableBool, TaskKey> IsMilestone;
```

## Voorbeelden

Toont hoe geschatte en/of mijlpaaltaak(en) te vinden.

```csharp
var prj = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(prj.RootTask, collector, 0);

// Itereer over de verzamelde taken.
foreach (var task in collector.Tasks)
{
    var estimated = task.Get(Tsk.IsEstimated).Value ? "Estimated" : "Non-Estimated";
    var milestone = task.Get(Tsk.IsMilestone).Value ? "Milestone" : "Non-Milestone";
    Console.WriteLine(task.Get(Tsk.Name) + " : " + estimated);
    Console.WriteLine(task.Get(Tsk.Name) + " : " + milestone);
}
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


