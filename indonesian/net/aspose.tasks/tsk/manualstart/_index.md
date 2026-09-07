---
title: "Tsk.ManualStart"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Menentukan awal yang dijadwalkan secara manual untuk sebuah tugas."
type: docs
weight: 800
url: /id/net/aspose.tasks/tsk/manualstart/
---
## Tsk.ManualStart field

Mendefinisikan mulai yang dijadwalkan secara manual untuk sebuah tugas.

```csharp
public static readonly Key<DateTime, TaskKey> ManualStart;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.ManualStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Manual Start: " + task.Get(Tsk.ManualStart));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


