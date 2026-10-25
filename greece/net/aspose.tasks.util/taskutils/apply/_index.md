---
title: "TaskUtils.Apply"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "TaskUtils μέθοδος. Εφαρμόζει τον καθορισμένο αλγόριθμο σε κάθε εργασία ενός δέντρου"
type: docs
weight: 10
url: /el/net/aspose.tasks.util/taskutils/apply/
---
## TaskUtils.Apply method

Εφαρμόζει τον καθορισμένο αλγόριθμο σε κάθε εργασία ενός δέντρου.

```csharp
public static void Apply(Task root, ITreeAlgorithm<Task> alg, int level)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| root | Εργασία | Ρίζα του δέντρου |
| alg | ITreeAlgorithm`1 | Εφαρμοσμένος αλγόριθμος. |
| επίπεδο | Int32 | Επίπεδο της ρίζας εργασίας. |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με έναν αλγόριθμο δέντρου.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// συλλέξτε όλες τις εργασίες του έργου
var coll = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, coll, 0);

// εργαστείτε με τις εργασίες όπως με μια απλή λίστα
foreach (var task in coll.Tasks)
{
    Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
}
```

### Δείτε επίσης

* class [Task](../../../aspose.tasks/task/)
* interface [ITreeAlgorithm&lt;T&gt;](../../itreealgorithm-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


