---
title: "Tsk.FinishVariance"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Waktu yang mewakili perbedaan antara tanggal selesai dasar sebuah tugas atau penugasan dan tanggal selesai saat ini"
type: docs
weight: 420
url: /id/net/aspose.tasks/tsk/finishvariance/
---
## Tsk.FinishVariance field

Waktu yang mewakili selisih antara tanggal selesai dasar sebuah tugas atau penugasan dan tanggal selesai saat ini.

```csharp
public static readonly Key<Duration, TaskKey> FinishVariance;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.FinishVariance.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FinishVariance, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Finish Variance: " + task.Get(Tsk.FinishVariance));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


