---
title: "Κλάση ChildTasksCollector"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Util.ChildTasksCollector κλάση. Συλλέγει όλες τις υποεργασίες"
type: docs
weight: 2690
url: /el/net/aspose.tasks.util/childtaskscollector/
---
## ChildTasksCollector class

Συλλέγει όλες τις υποεργασίες.

```csharp
public class ChildTasksCollector : TreeAlgorithmBase<Task>
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [ChildTasksCollector](childtaskscollector/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `ChildTasksCollector`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Tasks](../../aspose.tasks.util/childtaskscollector/tasks/) { get; } | Λαμβάνει μια λίστα με τα συλλεγμένα αντικείμενα-παιδιά (tasks). |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| override [Alg](../../aspose.tasks.util/childtaskscollector/alg/)(Task, int) | Επεξεργάζεται το καθορισμένο αντικείμενο. |
| virtual [PostAlg](../../aspose.tasks.util/treealgorithmbase-1/postalg/)(Task, int) |  |
| virtual [PreAlg](../../aspose.tasks.util/treealgorithmbase-1/prealg/)(Task, int) |  |

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

* class [TreeAlgorithmBase&lt;T&gt;](../treealgorithmbase-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


