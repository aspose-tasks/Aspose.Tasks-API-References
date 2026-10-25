---
title: "Tsk.OutlineLevel"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Το επίπεδο περιγράμματος μιας εργασίας"
type: docs
weight: 840
url: /el/net/aspose.tasks/tsk/outlinelevel/
---
## Tsk.OutlineLevel field

Το επίπεδο περιγράμματος μιας εργασίας.

```csharp
public static readonly Key<int, TaskKey> OutlineLevel;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις ιδιότητες περιγράμματος της εργασίας.

```csharp
var project = new Project(DataDir + "TaskOutlineProperties.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Αναλύστε όλες τις συλλεγμένες εργασίες
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name) + " - Outline Level : " + task.Get(Tsk.OutlineLevel));
    Console.WriteLine(task.Get(Tsk.Name) + " - Outline Number : " + task.Get(Tsk.OutlineNumber));
}
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


