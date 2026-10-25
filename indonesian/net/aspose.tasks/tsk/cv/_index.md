---
title: "Tsk.CV"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Perbedaan antara biaya dasar dan total biaya untuk sebuah tugas. Cost Variance  Cost  Baseline Cost"
type: docs
weight: 260
url: /id/net/aspose.tasks/tsk/cv/
---
## Tsk.CV field

Selisih antara biaya dasar dan total biaya untuk sebuah tugas. Variansi Biaya = Biaya - Biaya Dasar

```csharp
public static readonly Key<double, TaskKey> CV;
```

## Contoh

Menampilkan cara membaca nilai biaya tugas.

```csharp
var project = new Project(DataDir + "ResourceAssignmentCosts.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

foreach (var task in collector.Tasks)
{
    Console.WriteLine("Cost: " + task.Get(Tsk.Cost));
    Console.WriteLine("ACWP: " + task.Get(Tsk.ACWP));
    Console.WriteLine("BCWP: " + task.Get(Tsk.BCWP));
    Console.WriteLine("BCWS: " + task.Get(Tsk.BCWS));

    // CV = BCWP - ACWP
    Console.WriteLine("CV: " + task.Get(Tsk.CV));
    Console.WriteLine();
}
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


