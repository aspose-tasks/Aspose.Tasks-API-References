---
title: "Tsk.PercentComplete"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Status terkini sebuah tugas yang dinyatakan sebagai persentase durasi tugas yang telah selesai"
type: docs
weight: 880
url: /id/net/aspose.tasks/tsk/percentcomplete/
---
## Tsk.PercentComplete field

Status terkini tugas, dinyatakan sebagai persentase durasi tugas yang telah selesai.

```csharp
public static readonly Key<int, TaskKey> PercentComplete;
```

## Contoh

Menampilkan cara mengubah kemajuan tugas dengan memperbarui persentase penyelesaian tugas.

```csharp
var project = new Project();
Console.WriteLine("Project Calculation mode is Automatic: {0}", project.CalculationMode.Equals(CalculationMode.Automatic));

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(2));
task.Set(Tsk.PercentComplete, 50);

// Akses tugas dan tampilkan persentase penyelesaian
foreach (var tsk in project.RootTask.Children)
{
    Console.WriteLine(tsk.Get(Tsk.PercentComplete));
    Console.WriteLine(tsk.Get(Tsk.PercentWorkComplete));
    Console.WriteLine(tsk.Get(Tsk.PhysicalPercentComplete));
}
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


