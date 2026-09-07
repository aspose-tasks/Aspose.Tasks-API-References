---
title: "Tsk.Work"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Total waktu yang dijadwalkan pada sebuah tugas untuk semua sumber daya yang ditugaskan"
type: docs
weight: 1150
url: /id/net/aspose.tasks/tsk/work/
---
## Tsk.Work field

Total waktu yang dijadwalkan pada tugas untuk semua sumber daya yang ditugaskan.

```csharp
public static readonly Key<Duration, TaskKey> Work;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.Work.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Work, project.GetWork(1));

Console.WriteLine("Work: " + task.Get(Tsk.Work));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


