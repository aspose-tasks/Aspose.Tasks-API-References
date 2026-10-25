---
title: "SplitPart.Equals"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος SplitPart. Συγκρίνει δύο τμήματα"
type: docs
weight: 30
url: /el/net/aspose.tasks/splitpart/equals/
---
## SplitPart.Equals method

Συγκρίνει δύο split parts.

```csharp
public override bool Equals(object obj)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| obj | Αντικείμενο | Αντικείμενο για σύγκριση. |

### Τιμή Επιστροφής

Αληθές εάν το καθορισμένο αντικείμενο είναι ίσο με το τρέχον αντικείμενο· διαφορετικά, ψευδές.

## Παραδείγματα

Εμφανίζει πώς να ελέγξετε την ισότητα των τμημάτων διαχωρισμού.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 3, 21, 17, 0, 0));

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.IsManual, false);
task.Set(Tsk.Start, new DateTime(2000, 3, 15, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(4));

var assignment = project.ResourceAssignments.Add(task, project.Resources.Add("Resource"));
assignment.Set(Asn.Start, new DateTime(2000, 3, 15, 8, 0, 0));
assignment.Set(Asn.Work, task.Get(Tsk.Work));
assignment.Set(Asn.Finish, new DateTime(2000, 3, 19, 17, 0, 0));

// πρέπει πρώτα να δημιουργήσετε δεδομένα χρονομετρικής ανάθεσης πόρων
assignment.TimephasedDataFromTaskDuration(project.Get(Prj.Calendar));
Console.WriteLine(assignment.Get(Asn.Finish));

// διαχωρίστε την εργασία.
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 17, 17, 0, 0), project.Get(Prj.Calendar));

// Η ισότητα των τμημάτων διαχωρισμού ελέγχεται σε σχέση με την έναρξη, το τέλος και το δείκτη των τμημάτων διαχωρισμού.
var part1 = task.SplitParts[0];
var part2 = task.SplitParts[1];
Console.WriteLine("Split Part 1 Start {0} Finish {1}", part1.Start, part1.Finish);
Console.WriteLine("Split Part 2 Start {0} Finish {1}", part2.Start, part2.Finish);
Console.WriteLine("Are split parts equal: " + part1.Equals(part2));
```

### Δείτε επίσης

* class [SplitPart](../)
* namespace [Aspose.Tasks](../../splitpart/)
* assembly [Aspose.Tasks](../../../)


