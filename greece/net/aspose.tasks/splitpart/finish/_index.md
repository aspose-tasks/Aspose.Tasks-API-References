---
title: "SplitPart.Finish"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα SplitPart. Λαμβάνει την ημερομηνία λήξης ενός SplitPart"
type: docs
weight: 10
url: /el/net/aspose.tasks/splitpart/finish/
---
## SplitPart.Finish property

Λαμβάνει την ημερομηνία λήξης ενός SplitPart.

```csharp
public DateTime Finish { get; }
```

## Παραδείγματα

Δείχνει πώς να εργαστείτε με τα split parts μιας διαχωρισμένης εργασίας.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 3, 21, 17, 0, 0));

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.IsManual, false);
task.Set(Tsk.Start, new DateTime(2000, 3, 15, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(3));

var assignment = project.ResourceAssignments.Add(task, project.Resources.Add("r1"));
assignment.Set(Asn.Start, new DateTime(2000, 3, 15, 8, 0, 0));
assignment.Set(Asn.Work, task.Get(Tsk.Work));
assignment.Set(Asn.Finish, new DateTime(2000, 3, 19, 17, 0, 0));

// πρέπει πρώτα να δημιουργήσετε δεδομένα χρονομετρικής ανάθεσης πόρων
assignment.TimephasedDataFromTaskDuration(project.Get(Prj.Calendar));

// διαχωρίστε την εργασία.
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 17, 17, 0, 0), project.Get(Prj.Calendar));

// επανάληψη πάνω από τα τμήματα διαίρεσης
Console.WriteLine("Number of split parts: " + task.SplitParts.Count);
foreach (var splitPart in task.SplitParts)
{
    Console.WriteLine("  Split Part Start: " + splitPart.Start);
    Console.WriteLine("  Split Part Finish: " + splitPart.Finish);
    Console.WriteLine();
}
```

### Δείτε επίσης

* class [SplitPart](../)
* namespace [Aspose.Tasks](../../splitpart/)
* assembly [Aspose.Tasks](../../../)


