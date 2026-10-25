---
title: "Κλάση TaskLinkCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.TaskLinkCollection κλάση. Αναπαριστά μια συλλογή από αντικείμενα Task"
type: docs
weight: 2420
url: /el/net/aspose.tasks/tasklinkcollection/
---
## TaskLinkCollection class

Αναπαριστά μια συλλογή από αντικείμενα [`Task`](../task/).

```csharp
public class TaskLinkCollection : IList<TaskLink>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../aspose.tasks/tasklinkcollection/count/) { get; } | Λαμβάνει τον αριθμό των αντικειμένων που περιέχονται σε αυτό το αντικείμενο `TaskLinkCollection`. |
| [Item](../../aspose.tasks/tasklinkcollection/item/) { get; set; } | Επιστρέφει ή ορίζει το στοιχείο στη συγκεκριμένη θέση. |
| [ParentProject](../../aspose.tasks/tasklinkcollection/parentproject/) { get; } | Λαμβάνει το γονικό έργο του αντικειμένου ResourceAssignmentCollection. γονικό [`Project`](../project/) για αυτό το αντικείμενο. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_3)(TaskLink) | Αυτή είναι η ψευδοεφαρμογή της μεθόδου Add του ICollection, η οποία μόνο ρίχνει NotSupportedException |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add)(Task, Task) | Επιστρέφει ένα στιγμιότυπο του Finish-Start [`TaskLink`](../tasklink/) που έχει προστεθεί στο αντικείμενο TaskLinkCollection. |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_1)(Task, Task, TaskLinkType) | Επιστρέφει ένα στιγμιότυπο του [`TaskLink`](../tasklink/) που έχει προστεθεί στο αντικείμενο TaskLinkCollection. |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_2)(Task, Task, TaskLinkType, Duration) | Επιστρέφει ένα στιγμιότυπο του [`TaskLink`](../tasklink/) που έχει προστεθεί στο αντικείμενο TaskLinkCollection. |
| [GetEnumerator](../../aspose.tasks/tasklinkcollection/getenumerator/)() | Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή. |
| [Remove](../../aspose.tasks/tasklinkcollection/remove/)(TaskLink) | Αφαιρεί τη σύνδεση εργασίας από ένα έργο. |
| [ToList](../../aspose.tasks/tasklinkcollection/tolist/)() | Μετατρέπει το αντικείμενο TaskLinkCollection σε λίστα αντικειμένων [`TaskLink`](../tasklink/). |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με συλλογές συνδέσεων εργασίας.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// λάβετε εργασίες
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// συνδέστε τις εργασίες
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// εκτυπώστε τις συνδέσεις μεταξύ των εργασιών
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// επεξεργαστείτε τη σύνδεση με πρόσβαση κατά δείκτη
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// αφαιρέστε όλες τις συνδέσεις εργασίας
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### Δείτε επίσης

* class [TaskLink](../tasklink/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


