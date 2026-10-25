---
title: "SplitPart.GetHashCode"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος SplitPart. Επιστρέφει μια τιμή κώδικα κατακερματισμού για το στιγμιότυπο της κλάσης SplitPart."
type: docs
weight: 40
url: /el/net/aspose.tasks/splitpart/gethashcode/
---
## SplitPart.GetHashCode method

Επιστρέφει μια τιμή κώδικα κατακερματισμού για το στιγμιότυπο της κλάσης [`SplitPart`](../).

```csharp
public override int GetHashCode()
```

### Τιμή Επιστροφής

επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το αντικείμενο.

## Παραδείγματα

Εμφανίζει πώς να αποκτήσετε έναν κώδικα κατακερματισμού ενός τμήματος διαχωρισμού.

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

// Η ισότητα των τμημάτων διαχωρισμού ελέγχεται σε σχέση με την έναρξη, το τέλος και το δείκτη των τμημάτων διαχωρισμού.
var part1 = task.SplitParts[0];
var part2 = task.SplitParts[1];

// Ο κώδικας κατακερματισμού ενός τμήματος διαχωρισμού βασίζεται στην έναρξη, το τέλος και το δείκτη ενός τμήματος διαχωρισμού.
Console.WriteLine("Split Part 1 Start {0} Finish {1} HashCode {2}", part1.Start, part1.Finish, part1.GetHashCode());
Console.WriteLine("Split Part 2 Start {0} Finish {1} HashCode {2}", part2.Start, part2.Finish, part2.GetHashCode());
```

### Δείτε επίσης

* class [SplitPart](../)
* namespace [Aspose.Tasks](../../splitpart/)
* assembly [Aspose.Tasks](../../../)


