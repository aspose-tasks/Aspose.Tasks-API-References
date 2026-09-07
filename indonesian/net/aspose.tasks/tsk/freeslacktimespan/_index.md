---
title: "Tsk.FreeSlackTimeSpan"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Waktu yang dapat ditunda sebuah tugas tanpa menunda tugas penerus apa pun."
type: docs
weight: 450
url: /id/net/aspose.tasks/tsk/freeslacktimespan/
---
## Tsk.FreeSlackTimeSpan field

Waktu yang dapat ditunda sebuah tugas tanpa menunda tugas penerus apa pun.

```csharp
public static readonly Key<TimeSpan, TaskKey> FreeSlackTimeSpan;
```

## Contoh

Menampilkan cara membaca properti Tsk.FreeSlackTimeSpan. Properti ini dihitung, jadi biasanya tidak perlu mengaturnya secara eksplisit.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Free Slack: " + task.Get(Tsk.FreeSlackTimeSpan));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


