---
title: "TaskLink.LagFormat"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "TaskLink ιδιότητα. Λαμβάνει ή ορίζει τη μορφή για την έκφραση της μορφής καθυστέρησης"
type: docs
weight: 30
url: /el/net/aspose.tasks/tasklink/lagformat/
---
## TaskLink.LagFormat property

Λαμβάνει ή ορίζει τη μορφή για την έκφραση της μορφής καθυστέρησης.

```csharp
public TimeUnitType LagFormat { get; set; }
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

* enum [TimeUnitType](../../timeunittype/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


