---
title: "Tsk.Duration"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Total rentang waktu kerja aktif untuk sebuah tugas sebagaimana dimasukkan atau dihitung oleh Microsoft Project berdasarkan tanggal mulai, tanggal selesai, kalender, dan faktor penjadwalan lainnya."
type: docs
weight: 300
url: /id/net/aspose.tasks/tsk/duration/
---
## Tsk.Duration field

Rentang total waktu kerja aktif untuk sebuah tugas sebagaimana dimasukkan atau dihitung oleh Microsoft Project berdasarkan tanggal mulai, tanggal selesai, kalender, dan faktor penjadwalan lainnya.

```csharp
public static readonly Key<Duration, TaskKey> Duration;
```

## Contoh

Menampilkan cara mengatur durasi tugas.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Start, new DateTime(2012, 8, 23, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.ActualStart, new DateTime(2012, 8, 23, 8, 0, 0));

project.Save(OutDir + "AddTaskDuration_out.xml", SaveFileFormat.Xml);
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


