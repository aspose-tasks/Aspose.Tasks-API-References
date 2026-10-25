---
title: "Tsk.FinishSlackTimeSpan"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Durasi antara tanggal Selesai Awal dan Selesai Akhir"
type: docs
weight: 400
url: /id/net/aspose.tasks/tsk/finishslacktimespan/
---
## Tsk.FinishSlackTimeSpan field

Durasi antara tanggal Selesai Awal dan Selesai Akhir.

```csharp
public static readonly Key<TimeSpan, TaskKey> FinishSlackTimeSpan;
```

## Contoh

Menampilkan cara membaca properti Tsk.FinishSlackTimeSpan. Properti ini dihitung, jadi biasanya tidak perlu mengaturnya secara eksplisit.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Finish Slack: " + task.Get(Tsk.FinishSlackTimeSpan));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


