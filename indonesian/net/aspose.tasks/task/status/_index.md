---
title: "Task.Status"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Task. Mendapatkan status tugas"
type: docs
weight: 1160
url: /id/net/aspose.tasks/task/status/
---
## Task.Status property

Mendapatkan status tugas.

```csharp
public TaskStatus Status { get; }
```

## Contoh

Menampilkan cara mendapatkan status tugas.

```csharp
var project = new Project(DataDir + "TaskPercentageCompletion.mpp");

// Tanggal status proyek harus diatur karena perhitungan status menggunakan tanggal status.
project.StatusDate = new DateTime(2010, 7, 9, 15, 0, 0);
foreach (var task in project.EnumerateAllChildTasks())
{
    Console.WriteLine("{0} - {1}", task.Name, task.Status);
}
```

### Lihat Juga

* enum [TaskStatus](../../taskstatus/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


