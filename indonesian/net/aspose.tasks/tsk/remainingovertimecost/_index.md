---
title: "Tsk.RemainingOvertimeCost"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Biaya lembur terjadwal yang tersisa untuk sebuah tugas."
type: docs
weight: 970
url: /id/net/aspose.tasks/tsk/remainingovertimecost/
---
## Tsk.RemainingOvertimeCost field

Biaya lembur terjadwal yang tersisa untuk sebuah tugas.

```csharp
public static readonly Key<decimal, TaskKey> RemainingOvertimeCost;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.RemainingOvertimeCost.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingOvertimeCost, 2m);

Console.WriteLine("Remaining Overtime Cost: " + task.Get(Tsk.RemainingOvertimeCost));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


