---
title: "TaskLink.PredTask"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "TaskLink properti. Mendapatkan atau mengatur tugas pendahulu"
type: docs
weight: 70
url: /id/net/aspose.tasks/tasklink/predtask/
---
## TaskLink.PredTask property

Mendapatkan atau mengatur tugas pendahulu.

```csharp
public Task PredTask { get; set; }
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


