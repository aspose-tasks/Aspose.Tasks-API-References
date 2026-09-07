---
title: "Tsk.TotalSlackTimeSpan"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Waktu tanggal selesai tugas dapat ditunda tanpa menunda tanggal selesai proyek."
type: docs
weight: 1090
url: /id/net/aspose.tasks/tsk/totalslacktimespan/
---
## Tsk.TotalSlackTimeSpan field

Waktu tanggal selesai tugas dapat ditunda tanpa menunda tanggal selesai proyek.

```csharp
public static readonly Key<TimeSpan, TaskKey> TotalSlackTimeSpan;
```

## Contoh

Menampilkan cara membaca properti Tsk.TotalSlackTimeSpan. Properti ini dihitung, jadi biasanya tidak perlu mengaturnya secara eksplisit.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Total Slack: " + task.Get(Tsk.TotalSlackTimeSpan));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


