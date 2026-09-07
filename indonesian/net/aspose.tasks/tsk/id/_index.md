---
title: "Tsk.Id"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Pengidentifikasi posisi sebuah tugas dalam daftar tugas"
type: docs
weight: 520
url: /id/net/aspose.tasks/tsk/id/
---
## Tsk.Id field

Pengidentifikasi posisi sebuah tugas dalam daftar tugas.

```csharp
public static readonly Key<int, TaskKey> Id;
```

## Contoh

Menampilkan cara membaca/menulis properti tugas.

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
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


