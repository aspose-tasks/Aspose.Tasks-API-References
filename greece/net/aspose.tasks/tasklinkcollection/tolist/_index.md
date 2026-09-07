---
title: "TaskLinkCollection.ToList"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος TaskLinkCollection. Μετατρέπει το αντικείμενο TaskLinkCollection σε λίστα αντικειμένων TaskLink"
type: docs
weight: 70
url: /el/net/aspose.tasks/tasklinkcollection/tolist/
---
## TaskLinkCollection.ToList method

Μετατρέπει το αντικείμενο TaskLinkCollection σε λίστα αντικειμένων [`TaskLink`](../../tasklink/).

```csharp
public List<TaskLink> ToList()
```

### Τιμή Επιστροφής

Λίστα αντικειμένων [`TaskLink`](../../tasklink/).

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

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)


