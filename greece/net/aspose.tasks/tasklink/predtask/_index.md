---
title: "TaskLink.PredTask"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "TaskLink ιδιότητα. Λαμβάνει ή ορίζει την προηγούμενη εργασία"
type: docs
weight: 70
url: /el/net/aspose.tasks/tasklink/predtask/
---
## TaskLink.PredTask property

Λαμβάνει ή ορίζει την εργασία προκάτοχο.

```csharp
public Task PredTask { get; set; }
```

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

* class [Task](../../task/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


