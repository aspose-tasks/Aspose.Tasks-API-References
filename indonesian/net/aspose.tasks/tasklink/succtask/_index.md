---
title: "TaskLink.SuccTask"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "TaskLink properti. Mendapatkan atau mengatur tugas penerus"
type: docs
weight: 80
url: /id/net/aspose.tasks/tasklink/succtask/
---
## TaskLink.SuccTask property

Mendapatkan atau mengatur tugas penerus.

```csharp
public Task SuccTask { get; set; }
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

* class [Task](../../task/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


