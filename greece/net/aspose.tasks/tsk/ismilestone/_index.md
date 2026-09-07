---
title: "Tsk.IsMilestone"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Tsk field. Καθορίζει αν μια εργασία είναι ορόσημο."
type: docs
weight: 630
url: /el/net/aspose.tasks/tsk/ismilestone/
---
## Tsk.IsMilestone field

Καθορίζει εάν μια εργασία είναι ορόσημο.

```csharp
public static readonly Key<NullableBool, TaskKey> IsMilestone;
```

## Παραδείγματα

Δείχνει πώς να βρείτε εκτιμώμενες και/ή εργασίες ορόσημου.

```csharp
var prj = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(prj.RootTask, collector, 0);

// Επανάληψη πάνω στις συλλεγμένες εργασίες.
foreach (var task in collector.Tasks)
{
    var estimated = task.Get(Tsk.IsEstimated).Value ? "Estimated" : "Non-Estimated";
    var milestone = task.Get(Tsk.IsMilestone).Value ? "Milestone" : "Non-Milestone";
    Console.WriteLine(task.Get(Tsk.Name) + " : " + estimated);
    Console.WriteLine(task.Get(Tsk.Name) + " : " + milestone);
}
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


