---
title: "Tsk.IsCritical"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Καθορίζει εάν μια εργασία βρίσκεται στην κρίσιμη διαδρομή"
type: docs
weight: 560
url: /el/net/aspose.tasks/tsk/iscritical/
---
## Tsk.IsCritical field

Καθορίζει εάν μια εργασία βρίσκεται στην κρίσιμη διαδρομή.

```csharp
public static readonly Key<NullableBool, TaskKey> IsCritical;
```

## Παραδείγματα

Δείχνει πώς να βρείτε κρίσιμες και/ή εργασίες με βάση την προσπάθεια.

```csharp
var project = new Project(DataDir + "CriticalEffortDrivenTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Αναλύστε όλες τις συλλεγμένες εργασίες
foreach (var task in collector.Tasks)
{
    var effortDriven = task.Get(Tsk.IsEffortDriven).Value ? "EffortDriven" : "Non-EffortDriven";
    var nonCritical = task.Get(Tsk.IsCritical).Value ? "Critical" : "Non-Critical";
    Console.WriteLine(task.Get(Tsk.Name) + " : " + effortDriven);
    Console.WriteLine(task.Get(Tsk.Name) + " : " + nonCritical);
}
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


