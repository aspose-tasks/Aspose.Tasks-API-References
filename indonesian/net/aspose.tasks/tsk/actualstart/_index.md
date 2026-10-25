---
title: "Tsk.ActualStart"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Tanggal dan waktu ketika sebuah tugas benar‑benar dimulai"
type: docs
weight: 80
url: /id/net/aspose.tasks/tsk/actualstart/
---
## Tsk.ActualStart field

Tanggal dan waktu ketika sebuah tugas sebenarnya dimulai.

```csharp
public static readonly Key<DateTime, TaskKey> ActualStart;
```

## Contoh

Menampilkan bahwa tanggal proyek direset dalam mode evaluasi.

```csharp
var project = new Project();

// buat tugas baru
var task1 = project.RootTask.Children.Add("Task1");
task1.Set(Tsk.ActualStart, new DateTime(2000, 2, 10, 8, 0, 0));
task1.Set(Tsk.ActualFinish, new DateTime(2000, 2, 10, 17, 0, 0));

var task2 = project.RootTask.Children.Add("Task2");
task2.Set(Tsk.ActualStart, new DateTime(2000, 2, 10, 8, 0, 0));
task2.Set(Tsk.ActualFinish, new DateTime(2000, 2, 10, 17, 0, 0));

project.Save(OutDir + "EvaluationDateTimeLimitations_out.xml", SaveFileFormat.Xml);
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


