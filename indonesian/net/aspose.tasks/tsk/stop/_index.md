---
title: "Tsk.Stop"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Tsk field. Tanggal yang mewakili akhir bagian aktual dari sebuah tugas"
type: docs
weight: 1060
url: /id/net/aspose.tasks/tsk/stop/
---
## Tsk.Stop field

Tanggal yang mewakili akhir bagian aktual dari sebuah tugas.

```csharp
public static readonly Key<DateTime, TaskKey> Stop;
```

## Contoh

Menampilkan cara membaca tanggal Stop/Resume tugas.

```csharp
var project = new Project(DataDir + "StopResumeDates.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Periksa tanggal Stop dan Resume untuk semua tugas
foreach (var task in collector.Tasks)
{
    if (task.Get(Tsk.Stop).ToShortDateString() == "1/1/2000")
    {
        Console.WriteLine("Stop: NA");
    }
    else
    {
        Console.WriteLine("Stop: " + task.Get(Tsk.Stop).ToShortDateString());
    }

    if (task.Get(Tsk.Resume).ToShortDateString() == "1/1/2000")
    {
        Console.WriteLine("Resume: NA");
    }
    else
    {
        Console.WriteLine("Resume: " + task.Get(Tsk.Resume).ToShortDateString());
    }
}
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


