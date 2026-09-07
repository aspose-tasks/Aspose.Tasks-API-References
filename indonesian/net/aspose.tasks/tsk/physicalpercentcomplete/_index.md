---
title: "Tsk.PhysicalPercentComplete"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Nilai persentase selesai yang dapat digunakan sebagai alternatif untuk menghitung biaya anggaran kerja yang dilakukan (BCWP)"
type: docs
weight: 900
url: /id/net/aspose.tasks/tsk/physicalpercentcomplete/
---
## Tsk.PhysicalPercentComplete field

Nilai persentase selesai yang dapat digunakan sebagai alternatif untuk menghitung biaya anggaran pekerjaan yang dilakukan (BCWP).

```csharp
public static readonly Key<int, TaskKey> PhysicalPercentComplete;
```

## Contoh

Menunjukkan cara membaca/menulis properti Tsk.PhysicalPercentComplete.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PhysicalPercentComplete, 10);

Console.WriteLine("Physical Percent Complete: " + task.Get(Tsk.PhysicalPercentComplete));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


