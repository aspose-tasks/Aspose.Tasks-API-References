---
title: "Tsk.ActualWork"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Tsk field. Jumlah pekerjaan yang telah selesai dilakukan oleh sumber daya yang ditugaskan ke tugas"
type: docs
weight: 90
url: /id/net/aspose.tasks/tsk/actualwork/
---
## Tsk.ActualWork field

Jumlah pekerjaan yang sudah dilakukan oleh sumber daya yang ditugaskan pada tugas.

```csharp
public static readonly Key<Duration, TaskKey> ActualWork;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.ActualWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualWork, project.GetWork(1));

Console.WriteLine("Actual Work: " + task.Get(Tsk.ActualWork));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


