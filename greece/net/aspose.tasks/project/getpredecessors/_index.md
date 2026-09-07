---
title: "Project.GetPredecessors"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Project. Επιστρέφει μια συλλογή από συνδέσμους εργασιών που είναι προκάτοχοι της καθορισμένης εργασίας"
type: docs
weight: 1120
url: /el/net/aspose.tasks/project/getpredecessors/
---
## Project.GetPredecessors method

Επιστρέφει μια συλλογή συνδέσμων εργασιών που είναι προγενέστεροι της συγκεκριμένης εργασίας.

```csharp
public TaskLinkCollection GetPredecessors(Task task)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| εργασία | Εργασία | Η εργασία για την οποία θα ληφθούν οι προκάτοχοι. |

### Τιμή Επιστροφής

Λίστα προκάτοχων [`TaskLink`](../../tasklink/).

## Παραδείγματα

Δείχνει πώς να λάβετε προκάτοχους για τη συγκεκριμένη εργασία.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");
var task = project.RootTask.Children.GetById(10);

var predecessors = project.GetPredecessors(task);

// Εμφανίστε τα ονόματα των εργασιών προκάτοχου και επακόλουθου
foreach (var predecessor in predecessors)
{
    Console.WriteLine("Predecessor " + predecessor.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor " + predecessor.SuccTask.Get(Tsk.Name));
}
```

### Δείτε επίσης

* class [TaskLinkCollection](../../tasklinkcollection/)
* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


