---
title: "Tsk.DurationVariance"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Perbedaan antara durasi baseline sebuah tugas dan total durasi perkiraan saat ini dari tugas tersebut."
type: docs
weight: 320
url: /id/net/aspose.tasks/tsk/durationvariance/
---
## Tsk.DurationVariance field

Selisih antara durasi dasar sebuah tugas dan total durasi (perkiraan saat ini) sebuah tugas.

```csharp
public static readonly Key<Duration, TaskKey> DurationVariance;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.DurationVariance.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DurationVariance, project.GetWork(1));

Console.WriteLine("Duration Variance: " + task.Get(Tsk.DurationVariance));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


