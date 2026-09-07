---
title: "Task.Status"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Task. Λαμβάνει την κατάσταση της εργασίας."
type: docs
weight: 1160
url: /el/net/aspose.tasks/task/status/
---
## Task.Status property

Λαμβάνει την κατάσταση της εργασίας.

```csharp
public TaskStatus Status { get; }
```

## Παραδείγματα

Δείχνει πώς να ληφθεί η κατάσταση της εργασίας.

```csharp
var project = new Project(DataDir + "TaskPercentageCompletion.mpp");

// Η ημερομηνία κατάστασης του έργου πρέπει να οριστεί επειδή ο υπολογισμός της κατάστασης χρησιμοποιεί την ημερομηνία κατάστασης.
project.StatusDate = new DateTime(2010, 7, 9, 15, 0, 0);
foreach (var task in project.EnumerateAllChildTasks())
{
    Console.WriteLine("{0} - {1}", task.Name, task.Status);
}
```

### Δείτε επίσης

* enum [TaskStatus](../../taskstatus/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


