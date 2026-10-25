---
title: "Tsk.Deadline"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Tsk field. Tanggal target yang menunjukkan kapan sebuah tugas harus diselesaikan"
type: docs
weight: 270
url: /id/net/aspose.tasks/tsk/deadline/
---
## Tsk.Deadline field

Tanggal target yang menunjukkan kapan sebuah tugas harus diselesaikan.

```csharp
public static readonly Key<DateTime, TaskKey> Deadline;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.Deadline.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Deadline, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Deadline: " + task.Get(Tsk.Deadline));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


