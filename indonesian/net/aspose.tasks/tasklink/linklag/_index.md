---
title: "TaskLink.LinkLag"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "TaskLink properti. Mendapatkan atau mengatur jeda dalam sepersepuluh menit atau persentase"
type: docs
weight: 40
url: /id/net/aspose.tasks/tasklink/linklag/
---
## TaskLink.LinkLag property

Mendapatkan atau mengatur lag dalam satu persepuluh menit atau persentase.

```csharp
public int LinkLag { get; set; }
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

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


