---
title: "Tsk.ManualFinish"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Menentukan penyelesaian yang dijadwalkan secara manual untuk sebuah tugas"
type: docs
weight: 790
url: /id/net/aspose.tasks/tsk/manualfinish/
---
## Tsk.ManualFinish field

Mendefinisikan penyelesaian yang dijadwalkan secara manual untuk sebuah tugas.

```csharp
public static readonly Key<DateTime, TaskKey> ManualFinish;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.ManualFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Manual Finish: " + task.Get(Tsk.ManualFinish));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


