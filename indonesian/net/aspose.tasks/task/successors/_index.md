---
title: "Task.Successors"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Task. Mendapatkan objek TaskCollection yang berisi semua penerus dari objek Task ini"
type: docs
weight: 1200
url: /id/net/aspose.tasks/task/successors/
---
## Task.Successors property

Mendapatkan objek [`TaskCollection`](../../taskcollection/) yang berisi semua penerus dari objek Task ini.

```csharp
public TaskCollection Successors { get; }
```

### Nilai Kembali

Instansi read-only dari kelas [`TaskCollection`](../../taskcollection/).

## Contoh

Menampilkan cara membaca penerus tugas.

```csharp
var project = new Project();
var pred = project.RootTask.Children.Add("Predecessor");
var succ = project.RootTask.Children.Add("Successor");

project.TaskLinks.Add(pred, succ);

foreach (var successor in pred.Successors)
{
    Console.WriteLine("{0} {1}", successor.Get(Tsk.Id), successor.Get(Tsk.Name));
}
```

### Lihat Juga

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


