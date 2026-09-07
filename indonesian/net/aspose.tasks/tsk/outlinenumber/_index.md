---
title: "Tsk.OutlineNumber"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Angka yang mewakili posisi sebuah tugas dalam struktur outline hierarkis"
type: docs
weight: 850
url: /id/net/aspose.tasks/tsk/outlinenumber/
---
## Tsk.OutlineNumber field

Angka yang mewakili posisi tugas dalam struktur outline hierarkis.

```csharp
public static readonly Key<string, TaskKey> OutlineNumber;
```

## Contoh

Menampilkan cara membaca properti outline tugas.

```csharp
var project = new Project(DataDir + "TaskOutlineProperties.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Mengurai semua tugas yang dikumpulkan
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name) + " - Outline Level : " + task.Get(Tsk.OutlineLevel));
    Console.WriteLine(task.Get(Tsk.Name) + " - Outline Number : " + task.Get(Tsk.OutlineNumber));
}
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


