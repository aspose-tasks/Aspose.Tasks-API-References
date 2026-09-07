---
title: "Tsk.WBS"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Κωδικοί δομής εργασίας WBS"
type: docs
weight: 1130
url: /el/net/aspose.tasks/tsk/wbs/
---
## Tsk.WBS field

Κωδικοί δομής ανάλυσης εργασίας (WBS).

```csharp
public static readonly Key<string, TaskKey> WBS;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τους κωδικούς WBS της εργασίας.

```csharp
var project = new Project(DataDir + "TaskWBS.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Αναλύστε όλες τις συλλεγμένες εργασίες
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.WBS));
    Console.WriteLine(task.Get(Tsk.WBSLevel));
}
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


