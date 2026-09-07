---
title: "Tsk.CostVariance"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Selisih antara biaya dasar dan total biaya untuk sumber daya atau penugasan tugas."
type: docs
weight: 240
url: /id/net/aspose.tasks/tsk/costvariance/
---
## Tsk.CostVariance field

Selisih antara biaya dasar dan total biaya untuk sebuah tugas, sumber daya, atau penugasan.

```csharp
public static readonly Key<double, TaskKey> CostVariance;
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


