---
title: "Tsk.StartVariance"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Waktu yang mewakili perbedaan antara tanggal mulai baseline sebuah tugas atau penugasan dan tanggal mulai yang dijadwalkan saat ini."
type: docs
weight: 1040
url: /id/net/aspose.tasks/tsk/startvariance/
---
## Tsk.StartVariance field

Waktu yang mewakili selisih antara tanggal mulai baseline sebuah tugas atau penugasan dan tanggal mulai yang dijadwalkan saat ini.

```csharp
public static readonly Key<Duration, TaskKey> StartVariance;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.StartVariance.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StartVariance, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Start Variance: " + task.Get(Tsk.StartVariance));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


