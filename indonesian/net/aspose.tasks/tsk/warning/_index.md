---
title: "Tsk.Warning"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Tsk field. Mewakili bendera yang menunjukkan bahwa tugas memiliki ketidaksesuaian jadwal"
type: docs
weight: 1120
url: /id/net/aspose.tasks/tsk/warning/
---
## Tsk.Warning field

Mewakili flag yang menunjukkan bahwa tugas memiliki ketidaksesuaian jadwal.

```csharp
public static readonly Key<bool, TaskKey> Warning;
```

## Contoh

Menampilkan cara membaca peringatan tugas.

```csharp
var project = new Project(DataDir + "schedule-conflict.mpp");
var task = project.RootTask.Children.GetById(1);
Console.WriteLine(task.Get(Tsk.Warning));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


