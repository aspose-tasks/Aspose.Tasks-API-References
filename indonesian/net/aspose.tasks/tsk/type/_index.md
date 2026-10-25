---
title: "Tsk.Type"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Tipe tugas."
type: docs
weight: 1100
url: /id/net/aspose.tasks/tsk/type/
---
## Tsk.Type field

Tipe tugas.

```csharp
public static readonly Key<TaskType, TaskKey> Type;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.Type.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Type, TaskType.FixedDuration);

Console.WriteLine("Type: " + task.Get(Tsk.Type));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskType](../../tasktype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


