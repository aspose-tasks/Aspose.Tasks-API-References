---
title: "ChildTasksCollector.ChildTasksCollector"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής ChildTasksCollector. Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης ChildTasksCollector"
type: docs
weight: 10
url: /el/net/aspose.tasks.util/childtaskscollector/childtaskscollector/
---
## ChildTasksCollector constructor

Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [`ChildTasksCollector`](../).

```csharp
public ChildTasksCollector()
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

* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


