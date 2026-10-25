---
title: "Tsk.ManualDuration"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Menentukan durasi yang dijadwalkan secara manual untuk sebuah tugas"
type: docs
weight: 780
url: /id/net/aspose.tasks/tsk/manualduration/
---
## Tsk.ManualDuration field

Mendefinisikan durasi yang dijadwalkan secara manual untuk sebuah tugas.

```csharp
public static readonly Key<Duration, TaskKey> ManualDuration;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.ManualDuration.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualDuration, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Manual Duration: " + task.Get(Tsk.ManualDuration));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


