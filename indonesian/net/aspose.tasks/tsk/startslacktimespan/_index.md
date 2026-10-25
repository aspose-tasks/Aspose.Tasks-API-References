---
title: "Tsk.StartSlackTimeSpan"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Durasi antara tanggal Mulai Awal dan Mulai Akhir"
type: docs
weight: 1020
url: /id/net/aspose.tasks/tsk/startslacktimespan/
---
## Tsk.StartSlackTimeSpan field

Durasi antara tanggal Early Start dan Late Start.

```csharp
public static readonly Key<TimeSpan, TaskKey> StartSlackTimeSpan;
```

## Contoh

Menampilkan cara membaca properti Tsk.StartSlackTimeSpan. Properti ini dihitung, jadi biasanya tidak perlu mengaturnya secara eksplisit.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Start Slack: " + task.Get(Tsk.StartSlackTimeSpan));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


