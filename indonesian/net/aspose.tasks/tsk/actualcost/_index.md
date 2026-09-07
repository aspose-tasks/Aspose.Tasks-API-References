---
title: "Tsk.ActualCost"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Biaya yang timbul untuk pekerjaan yang sudah dilakukan oleh sumber daya pada tugas mereka bersama dengan biaya lain yang tercatat terkait tugas tersebut"
type: docs
weight: 20
url: /id/net/aspose.tasks/tsk/actualcost/
---
## Tsk.ActualCost field

Biaya yang dikeluarkan untuk pekerjaan yang sudah dilakukan oleh sumber daya pada tugas mereka, bersama dengan biaya lain yang tercatat terkait dengan tugas tersebut.

```csharp
public static readonly Key<decimal, TaskKey> ActualCost;
```

## Contoh

Menampilkan cara membaca properti aktual tugas.

```csharp
var project = new Project(DataDir + "ActualTaskProperties.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Mengurai semua tugas yang dikumpulkan
foreach (var task in collector.Tasks)
{
    Console.WriteLine("Task Name : " + task.Get(Tsk.Name));
    Console.WriteLine("Actual Start: " + task.Get(Tsk.ActualStart).ToLongDateString());
    Console.WriteLine("Actual Finish: " + task.Get(Tsk.ActualFinish).ToLongDateString());
    Console.WriteLine("Actual Duration: " + task.Get(Tsk.ActualDuration).TimeSpan.Hours);
    Console.WriteLine("Actual Cost: " + task.Get(Tsk.ActualCost));
}
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


