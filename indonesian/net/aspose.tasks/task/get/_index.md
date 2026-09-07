---
title: "Task.Get"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Task. Mengembalikan nilai yang dipetakan ke properti dalam kontainer ini"
type: docs
weight: 1340
url: /id/net/aspose.tasks/task/get/
---
## Task.Get&lt;T&gt; method

Mengembalikan nilai yang dipetakan ke properti ini dalam kontainer ini.

```csharp
public T Get<T>(Key<T, TaskKey> key)
```

| Parameter | Deskripsi |
| --- | --- |
| T | tipe nilai yang dipetakan. |
| key | kunci properti yang ditentukan. [`Tsk`](../../tsk/) untuk mendapatkan kunci properti. |

### Nilai Kembali

nilai yang dipetakan ke properti dalam wadah ini.

## Contoh

Menampilkan cara mendapatkan/mengatur properti tugas.

```csharp
var project = new Project();

// Tambahkan tugas dan atur properti tugas
var task = project.RootTask.Children.Add();
task.Set(Tsk.Name, "Task1");
task.Set(Tsk.Start, new DateTime(2020, 3, 31, 8, 0, 0));
task.Set(Tsk.Finish, new DateTime(2020, 3, 31, 17, 0, 0));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Mengurai semua tugas yang dikumpulkan
foreach (var tsk in collector.Tasks)
{
    Console.WriteLine("Task Id: {0}", tsk.Get(Tsk.Id));
    Console.WriteLine("Task Uid: {0}", tsk.Get(Tsk.Uid));
    Console.WriteLine("Task Name: {0}", tsk.Get(Tsk.Name));
    Console.WriteLine("Task Start: {0}", tsk.Get(Tsk.Start));
    Console.WriteLine("Task Finish: {0}", tsk.Get(Tsk.Finish));
}
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


