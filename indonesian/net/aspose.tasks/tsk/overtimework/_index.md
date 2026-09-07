---
title: "Tsk.OvertimeWork"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Tsk field. Jumlah lembur yang dijadwalkan untuk dilakukan oleh semua sumber daya yang ditugaskan ke sebuah tugas"
type: docs
weight: 870
url: /id/net/aspose.tasks/tsk/overtimework/
---
## Tsk.OvertimeWork field

Jumlah lembur yang dijadwalkan untuk dilakukan oleh semua sumber daya yang ditugaskan ke sebuah tugas.

```csharp
public static readonly Key<Duration, TaskKey> OvertimeWork;
```

## Contoh

Menunjukkan cara membaca lembur tugas.

```csharp
var project = new Project(DataDir + "TaskOvertimes.mpp");

// Baca lembur dan persentase penyelesaian untuk tugas
foreach (var task in project.RootTask.Children)
{
    Console.WriteLine(task.Get(Tsk.OvertimeCost));
    Console.WriteLine(task.Get(Tsk.OvertimeWork));
    Console.WriteLine(task.Get(Tsk.PercentComplete));
    Console.WriteLine(task.Get(Tsk.PercentWorkComplete));
    Console.WriteLine(task.Get(Tsk.PhysicalPercentComplete));

    // Atur persentase selesai
    task.Set(Tsk.PercentComplete, 100);
}
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


