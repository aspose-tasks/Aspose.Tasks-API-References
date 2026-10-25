---
title: "TaskLink.LagFormat"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "TaskLink properti. Mendapatkan atau mengatur format untuk mengekspresikan format jeda"
type: docs
weight: 30
url: /id/net/aspose.tasks/tasklink/lagformat/
---
## TaskLink.LagFormat property

Mendapatkan atau mengatur format untuk mengekspresikan format lag.

```csharp
public TimeUnitType LagFormat { get; set; }
```

## Contoh

Menampilkan cara membaca tautan tugas proyek.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

// Tampilkan nama tugas pendahulu dan penerus
foreach (var taskLink in project.TaskLinks)
{
    Console.WriteLine("Predecessor: " + taskLink.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor: " + taskLink.SuccTask.Get(Tsk.Name));
    Console.WriteLine("Lag Format: " + taskLink.LagFormat);
    Console.WriteLine("Link Lag: " + taskLink.LinkLag);
    Console.WriteLine();
}
```

### Lihat Juga

* enum [TimeUnitType](../../timeunittype/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


