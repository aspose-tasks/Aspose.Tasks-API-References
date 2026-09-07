---
title: "Task.ParentProject"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Task. Λαμβάνει το γονικό έργο μιας εργασίας."
type: docs
weight: 930
url: /el/net/aspose.tasks/task/parentproject/
---
## Task.ParentProject property

Λαμβάνει το γονικό έργο μιας εργασίας.

```csharp
public Project ParentProject { get; }
```

## Παρατηρήσεις

Καλέστε το Project.UpdateReferences για να ενημερώσετε αυτές τις ιδιότητες.

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε το γονικό έργο μιας εργασίας.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Parent");

// Ορίστε διάρκεια για την εργασία χρησιμοποιώντας τον προεπιλεγμένο τύπο μονάδας χρόνου του έργου.
task.Set(Tsk.Duration, task.ParentProject.GetDuration(1));

Console.WriteLine(task.Get(Tsk.Duration));
```

### Δείτε επίσης

* class [Project](../../project/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


