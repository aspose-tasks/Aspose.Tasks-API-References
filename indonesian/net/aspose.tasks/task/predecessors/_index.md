---
title: "Task.Predecessors"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Task. Mendapatkan objek TaskCollection yang berisi semua pendahulu dari objek Task ini"
type: docs
weight: 980
url: /id/net/aspose.tasks/task/predecessors/
---
## Task.Predecessors property

Mendapatkan objek [`TaskCollection`](../../taskcollection/) yang berisi semua pendahulu dari objek Task ini.

```csharp
public TaskCollection Predecessors { get; }
```

### Nilai Kembali

Instansi read-only dari kelas [`TaskCollection`](../../taskcollection/).

## Contoh

Menampilkan cara membaca pendahulu tugas.

```csharp
var project = new Project();
var pred = project.RootTask.Children.Add("Predecessor");
var succ = project.RootTask.Children.Add("Successor");

project.TaskLinks.Add(pred, succ);

foreach (var predecessor in succ.Predecessors)
{
    Console.WriteLine("{0} {1}", predecessor.Get(Tsk.Id), predecessor.Get(Tsk.Name));
}
```

### Lihat Juga

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


