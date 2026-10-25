---
title: "Tsk.ConstraintDate"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Tanggal spesifik yang terkait dengan tipe kendala."
type: docs
weight: 200
url: /id/net/aspose.tasks/tsk/constraintdate/
---
## Tsk.ConstraintDate field

Tanggal spesifik yang terkait dengan tipe kendala.

```csharp
public static readonly Key<DateTime, TaskKey> ConstraintDate;
```

## Contoh

Menampilkan cara mendapatkan/mengatur sebuah kendala untuk sebuah tugas.

```csharp
var project = new Project(DataDir + "ConstraintAsLateAsPossible.mpp");

// Atur kendala As Late As Possible untuk tugas dengan Id 11
var newTask = project.RootTask.Children.GetById(11);
newTask.Set(Tsk.ConstraintType, ConstraintType.AsLateAsPossible);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Mengurai semua tugas yang dikumpulkan
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.ConstraintType).ToString());
    Console.WriteLine(task.Get(Tsk.ConstraintDate).ToShortDateString() == "1/1/2000" ? "NA" : task.Get(Tsk.ConstraintDate).ToShortDateString());
}

SaveOptions options = new PdfSaveOptions
{
    StartDate = project.Get(Prj.StartDate),
    Timescale = Timescale.ThirdsOfMonths
};

project.Save(OutDir + "SetConstraintAsLateAsPossible_out.pdf", options);
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


