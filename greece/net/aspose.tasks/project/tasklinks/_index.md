---
title: "Project.TaskLinks"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Project. Λαμβάνει το αντικείμενο TaskLinkCollection"
type: docs
weight: 930
url: /el/net/aspose.tasks/project/tasklinks/
---
## Project.TaskLinks property

Λαμβάνει το αντικείμενο [`TaskLinkCollection`](../../tasklinkcollection/).

```csharp
public TaskLinkCollection TaskLinks { get; }
```

## Παραδείγματα

Δείχνει πώς να δημιουργήσετε συνδέσμους εργασιών.

```csharp
var project = new Project();

// Προσθέστε νέες εργασίες
var pred = project.RootTask.Children.Add("Task 1");
var succ = project.RootTask.Children.Add("Task 2");

// Συνδέστε εργασίες
project.TaskLinks.Add(pred, succ);

foreach (var link in project.TaskLinks)
{
    Console.WriteLine("Predecessor Task: " + link.PredTask);
    Console.WriteLine("Successor Task: " + link.SuccTask);
    Console.WriteLine("LagFormat: " + link.LagFormat);
    Console.WriteLine("LinkType: " + link.LinkType);
    Console.WriteLine("LinkLag: " + link.LinkLag);
    Console.WriteLine("CrossProjectName: " + link.CrossProjectName);
    Console.WriteLine("IsCrossProject: " + link.IsCrossProject);
}
```

### Δείτε επίσης

* class [TaskLinkCollection](../../tasklinkcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


