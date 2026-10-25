---
title: "Tsk.LateStart"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Tanggal terbaru yang dapat dimulai tugas tanpa menunda penyelesaian proyek"
type: docs
weight: 740
url: /id/net/aspose.tasks/tsk/latestart/
---
## Tsk.LateStart field

Tanggal terakhir yang dapat dimulai oleh tugas tanpa menunda penyelesaian proyek.

```csharp
public static readonly Key<DateTime, TaskKey> LateStart;
```

## Contoh

Menunjukkan cara membaca/menulis properti Tsk.LateStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LateStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Late Start: " + task.Get(Tsk.LateStart));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


