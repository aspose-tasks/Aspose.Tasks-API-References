---
title: "Κλάση SplitPart"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Η κλάση Aspose.Tasks.SplitPart. Αντιπροσωπεύει ένα τμήμα εργασίας. Το SplitPart είναι μέλος της συλλογής SplitParts των εργασιών."
type: docs
weight: 2290
url: /el/net/aspose.tasks/splitpart/
---
## SplitPart class

Αντιπροσωπεύει ένα τμήμα εργασίας. Το SplitPart είναι μέλος της συλλογής SplitParts της εργασίας.

```csharp
public class SplitPart
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Finish](../../aspose.tasks/splitpart/finish/) { get; } | Λαμβάνει την ημερομηνία λήξης ενός SplitPart. |
| [Start](../../aspose.tasks/splitpart/start/) { get; } | Λαμβάνει την ημερομηνία έναρξης ενός SplitPart. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| override [Equals](../../aspose.tasks/splitpart/equals/)(object) | Συγκρίνει δύο split parts. |
| override [GetHashCode](../../aspose.tasks/splitpart/gethashcode/)() | Επιστρέφει μια τιμή κώδικα κατακερματισμού για το παράδειγμα της κλάσης `SplitPart`. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


