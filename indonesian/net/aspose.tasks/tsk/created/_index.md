---
title: "Tsk.Created"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Tanggal ketika tugas dibuat."
type: docs
weight: 250
url: /id/net/aspose.tasks/tsk/created/
---
## Tsk.Created field

Tanggal ketika sebuah tugas dibuat.

```csharp
public static readonly Key<DateTime, TaskKey> Created;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.Created.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Created, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Created: " + task.Get(Tsk.Created));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


