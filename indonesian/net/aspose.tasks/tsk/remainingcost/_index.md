---
title: "Tsk.RemainingCost"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Tsk field. Biaya terjadwal yang tersisa yang akan dikeluarkan dalam menyelesaikan pekerjaan terjadwal yang tersisa"
type: docs
weight: 950
url: /id/net/aspose.tasks/tsk/remainingcost/
---
## Tsk.RemainingCost field

Biaya terjadwal yang tersisa yang akan timbul dalam menyelesaikan pekerjaan terjadwal yang tersisa.

```csharp
public static readonly Key<decimal, TaskKey> RemainingCost;
```

## Contoh

Menampilkan cara membaca biaya tugas.

```csharp
var project = new Project();

// Tambahkan tugas dan tetapkan biaya
var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Cost, 800);

// Tampilkan properti terkait biaya dari tugas
Console.WriteLine(task.Get(Tsk.RemainingCost));
Console.WriteLine(task.Get(Tsk.FixedCost));
Console.WriteLine(task.Get(Tsk.CostVariance));
Console.WriteLine(project.RootTask.Get(Tsk.Cost));
Console.WriteLine(project.RootTask.Get(Tsk.FixedCost));
Console.WriteLine(project.RootTask.Get(Tsk.RemainingCost));
Console.WriteLine(project.RootTask.Get(Tsk.CostVariance));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


