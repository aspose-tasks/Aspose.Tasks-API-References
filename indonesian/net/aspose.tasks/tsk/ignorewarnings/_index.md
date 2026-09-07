---
title: "Tsk.IgnoreWarnings"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Menunjukkan apakah menyembunyikan indikator peringatan konflik jadwal di Microsoft Project"
type: docs
weight: 540
url: /id/net/aspose.tasks/tsk/ignorewarnings/
---
## Tsk.IgnoreWarnings field

Menunjukkan apakah harus menyembunyikan indikator peringatan konflik jadwal di Microsoft Project.

```csharp
public static readonly Key<bool, TaskKey> IgnoreWarnings;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.IgnoreWarnings.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IgnoreWarnings, true);

Console.WriteLine("Ignore Warnings: " + task.Get(Tsk.IgnoreWarnings));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


