---
title: "Tsk.ActualOvertimeWork"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Tsk field. Jumlah kerja lembur aktual yang sudah dilakukan oleh sumber daya yang ditugaskan pada tugas"
type: docs
weight: 60
url: /id/net/aspose.tasks/tsk/actualovertimework/
---
## Tsk.ActualOvertimeWork field

Jumlah aktual pekerjaan lembur yang sudah dilakukan oleh sumber daya yang ditugaskan pada tugas.

```csharp
public static readonly Key<Duration, TaskKey> ActualOvertimeWork;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.ActualOvertimeWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeWork, project.GetWork(1));

Console.WriteLine("Actual Overtime Work: " + task.Get(Tsk.ActualOvertimeWork));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


