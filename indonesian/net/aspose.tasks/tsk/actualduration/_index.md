---
title: "Tsk.ActualDuration"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Rentang waktu kerja aktual untuk sebuah tugas berdasarkan durasi yang dijadwalkan dan pekerjaan yang tersisa saat ini atau persentase penyelesaian."
type: docs
weight: 30
url: /id/net/aspose.tasks/tsk/actualduration/
---
## Tsk.ActualDuration field

Rentang waktu kerja aktual untuk sebuah tugas, berdasarkan durasi terjadwal dan pekerjaan yang tersisa saat ini atau persentase penyelesaian.

```csharp
public static readonly Key<Duration, TaskKey> ActualDuration;
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
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


