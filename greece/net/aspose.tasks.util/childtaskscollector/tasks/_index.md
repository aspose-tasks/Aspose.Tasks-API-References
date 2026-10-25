---
title: "ChildTasksCollector.Tasks"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ChildTasksCollector. Λαμβάνει μια λίστα με τις εργασίες των συλλεγμένων αντικειμένων-παιδιών"
type: docs
weight: 20
url: /el/net/aspose.tasks.util/childtaskscollector/tasks/
---
## ChildTasksCollector.Tasks property

Λαμβάνει μια λίστα με τα συλλεγμένα αντικείμενα-παιδιά (tasks).

```csharp
public List<Task> Tasks { get; }
```

## Παραδείγματα

Δείχνει πώς να επαναλάβετε όλες τις εργασίες σε ένα έργο ως απλή λίστα.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Αναλύστε όλες τις συλλεγμένες εργασίες
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### Δείτε επίσης

* class [Task](../../../aspose.tasks/task/)
* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


