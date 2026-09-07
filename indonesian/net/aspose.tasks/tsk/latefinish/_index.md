---
title: "Tsk.LateFinish"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Tanggal terbaru yang dapat menyelesaikan tugas tanpa menunda penyelesaian proyek"
type: docs
weight: 730
url: /id/net/aspose.tasks/tsk/latefinish/
---
## Tsk.LateFinish field

Tanggal terakhir yang dapat diselesaikan oleh tugas tanpa menunda penyelesaian proyek.

```csharp
public static readonly Key<DateTime, TaskKey> LateFinish;
```

## Contoh

Menunjukkan cara membaca/menulis properti Tsk.LateFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LateFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Late Finish: " + task.Get(Tsk.LateFinish));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


