---
title: "Project.GetPredecessors"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Project. Mengembalikan koleksi tautan tugas yang merupakan pendahulu tugas yang ditentukan"
type: docs
weight: 1120
url: /id/net/aspose.tasks/project/getpredecessors/
---
## Project.GetPredecessors method

Mengembalikan koleksi tautan tugas yang merupakan pendahulu tugas yang ditentukan.

```csharp
public TaskLinkCollection GetPredecessors(Task task)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tugas | Tugas | Tugas untuk mendapatkan pendahulunya. |

### Nilai Kembali

Daftar pendahulu [`TaskLink`](../../tasklink/).

## Contoh

Menampilkan cara mendapatkan pendahulu untuk tugas tertentu.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");
var task = project.RootTask.Children.GetById(10);

var predecessors = project.GetPredecessors(task);

// Tampilkan nama tugas pendahulu dan penerus
foreach (var predecessor in predecessors)
{
    Console.WriteLine("Predecessor " + predecessor.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor " + predecessor.SuccTask.Get(Tsk.Name));
}
```

### Lihat Juga

* class [TaskLinkCollection](../../tasklinkcollection/)
* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


