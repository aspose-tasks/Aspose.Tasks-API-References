---
title: "TaskLink.LinkType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "TaskLink ιδιότητα. Λαμβάνει ή ορίζει τον τύπο ενός συνδέσμου"
type: docs
weight: 60
url: /el/net/aspose.tasks/tasklink/linktype/
---
## TaskLink.LinkType property

Λαμβάνει ή ορίζει τον τύπο ενός συνδέσμου.

```csharp
public TaskLinkType LinkType { get; set; }
```

## Παραδείγματα

Δείχνει πώς να λάβετε/ορίσετε έναν τύπο σύνδεσης ενός συνδέσμου εργασίας.

```csharp
var project = new Project();

// Προσθέστε νέες εργασίες
var pred = project.RootTask.Children.Add("Task 1");
var succ = project.RootTask.Children.Add("Task 2");

// Συνδέστε εργασίες με τύπο σύνδεσης ορισμένο σε Έναρξη-σε-Έναρξη
var newLink = project.TaskLinks.Add(pred, succ);
newLink.LinkType = TaskLinkType.StartToStart;

foreach (var link in project.TaskLinks)
{
    Console.WriteLine("Task Link Type: " + link.LinkType.ToString());
}
```

### Δείτε επίσης

* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


