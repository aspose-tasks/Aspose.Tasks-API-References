---
title: "Κλάση TaskLink"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.TaskLink κλάση. Αντιπροσωπεύει έναν σύνδεσμο προκάτοχου"
type: docs
weight: 2410
url: /el/net/aspose.tasks/tasklink/
---
## TaskLink class

Αντιπροσωπεύει έναν σύνδεσμο προκάτοχου.

```csharp
public sealed class TaskLink : IEquatable<TaskLink>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [CrossProjectName](../../aspose.tasks/tasklink/crossprojectname/) { get; set; } | Λαμβάνει ή ορίζει το εξωτερικό έργο προκάτοχο. |
| [IsCrossProject](../../aspose.tasks/tasklink/iscrossproject/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν ένας προκάτοχος αποτελεί μέρος άλλου έργου. |
| [LagFormat](../../aspose.tasks/tasklink/lagformat/) { get; set; } | Λαμβάνει ή ορίζει τη μορφή για την έκφραση της μορφής καθυστέρησης. |
| [LinkLag](../../aspose.tasks/tasklink/linklag/) { get; set; } | Λαμβάνει ή ορίζει την καθυστέρηση σε δέκατα του λεπτού ή ποσοστό. |
| [LinkLagTimeSpan](../../aspose.tasks/tasklink/linklagtimespan/) { get; set; } | Λαμβάνει ή ορίζει τη διάρκεια της καθυστέρησης, ανάλογα με το LagFormat. |
| [LinkType](../../aspose.tasks/tasklink/linktype/) { get; set; } | Λαμβάνει ή ορίζει τον τύπο ενός συνδέσμου. |
| [PredTask](../../aspose.tasks/tasklink/predtask/) { get; set; } | Λαμβάνει ή ορίζει την εργασία προκάτοχο. |
| [SuccTask](../../aspose.tasks/tasklink/succtask/) { get; set; } | Λαμβάνει ή ορίζει την εργασία επακόλουθο. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| override [Equals](../../aspose.tasks/tasklink/equals/#equals_1)(object) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| [Equals](../../aspose.tasks/tasklink/equals/#equals)(TaskLink) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| override [GetHashCode](../../aspose.tasks/tasklink/gethashcode/)() | Επιστρέφει μια τιμή κώδικα κατακερματισμού για το στιγμιότυπο της κλάσης `TaskLink`. |
| override [ToString](../../aspose.tasks/tasklink/tostring/)() | Επιστρέφει την αναπαράσταση συμβολοσειράς ενός TaskLink. Οι ακριβείς λεπτομέρειες της αναπαράστασης δεν καθορίζονται και ενδέχεται να αλλάξουν. |

## Παραδείγματα

Δείχνει πώς να διαβάσετε τους συνδέσμους εργασιών του έργου.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

// Εμφανίστε τα ονόματα των εργασιών προκάτοχου και επακόλουθου
foreach (var taskLink in project.TaskLinks)
{
    Console.WriteLine("Predecessor: " + taskLink.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor: " + taskLink.SuccTask.Get(Tsk.Name));
    Console.WriteLine("Lag Format: " + taskLink.LagFormat);
    Console.WriteLine("Link Lag: " + taskLink.LinkLag);
    Console.WriteLine();
}
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


