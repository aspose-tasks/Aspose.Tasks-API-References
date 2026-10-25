---
title: "Tsk.RemainingDuration"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Tsk field. Waktu yang diperlukan untuk menyelesaikan bagian tugas yang belum selesai"
type: docs
weight: 960
url: /id/net/aspose.tasks/tsk/remainingduration/
---
## Tsk.RemainingDuration field

Waktu yang diperlukan untuk menyelesaikan bagian tugas yang belum selesai.

```csharp
public static readonly Key<Duration, TaskKey> RemainingDuration;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.RemainingDuration.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingDuration, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Remaining Duration: " + task.Get(Tsk.RemainingDuration));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


