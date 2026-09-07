---
title: "Tsk.OvertimeCost"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Total biaya lembur untuk sebuah tugas bagi sebuah sumber daya pada semua tugas yang ditugaskan atau untuk penugasan sumber daya"
type: docs
weight: 860
url: /id/net/aspose.tasks/tsk/overtimecost/
---
## Tsk.OvertimeCost field

Total biaya lembur untuk sebuah tugas, untuk sebuah sumber daya pada semua tugas yang ditugaskan, atau untuk penugasan sumber daya.

```csharp
public static readonly Key<decimal, TaskKey> OvertimeCost;
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
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


