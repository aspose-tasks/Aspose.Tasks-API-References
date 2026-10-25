---
title: "Tsk.WorkVariance"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Tsk field. Perbedaan antara pekerjaan dasar sebuah tugas dan pekerjaan yang saat ini dijadwalkan"
type: docs
weight: 1160
url: /id/net/aspose.tasks/tsk/workvariance/
---
## Tsk.WorkVariance field

Selisih antara pekerjaan baseline sebuah tugas dan pekerjaan yang dijadwalkan saat ini.

```csharp
public static readonly Key<Duration, TaskKey> WorkVariance;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.WorkVariance.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.WorkVariance, project.GetDuration(1));

Console.WriteLine("Work Variance: " + task.Get(Tsk.WorkVariance));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


