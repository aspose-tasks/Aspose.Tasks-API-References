---
title: "Enum TaskLinkType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.TaskLinkType enum. Καθορίζει τον τύπο της εξάρτησης εργασιών."
type: docs
weight: 2440
url: /el/net/aspose.tasks/tasklinktype/
---
## TaskLinkType enumeration

Καθορίζει τον τύπο εξάρτησης εργασιών.

```csharp
public enum TaskLinkType
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| FinishToFinish | `0` | Σχέση Τερματισμού-Τερματισμού |
| FinishToStart | `1` | Σχέση Τερματισμού-Έναρξης |
| StartToFinish | `2` | Σχέση Έναρξης-Τερματισμού |
| StartToStart | `3` | Σχέση Έναρξης-Έναρξης |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


