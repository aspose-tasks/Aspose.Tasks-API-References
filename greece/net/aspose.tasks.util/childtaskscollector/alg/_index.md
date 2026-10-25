---
title: "ChildTasksCollector.Alg"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ChildTasksCollector. Επεξεργάζεται το καθορισμένο αντικείμενο"
type: docs
weight: 30
url: /el/net/aspose.tasks.util/childtaskscollector/alg/
---
## ChildTasksCollector.Alg method

Επεξεργάζεται το καθορισμένο αντικείμενο.

```csharp
public override void Alg(Task el, int level)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| el | Εργασία | Αντικείμενο προς επεξεργασία. |
| επίπεδο | Int32 | Επίπεδο κόμβου δέντρου. |

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


