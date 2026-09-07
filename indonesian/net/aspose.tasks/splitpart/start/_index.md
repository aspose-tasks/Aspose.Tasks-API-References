---
title: "SplitPart.Start"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti SplitPart. Mendapatkan tanggal mulai dari sebuah SplitPart"
type: docs
weight: 20
url: /id/net/aspose.tasks/splitpart/start/
---
## SplitPart.Start property

Mendapatkan tanggal mulai dari sebuah SplitPart.

```csharp
public DateTime Start { get; }
```

## Contoh

Menampilkan cara bekerja dengan split part dari tugas yang terpecah.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 3, 21, 17, 0, 0));

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.IsManual, false);
task.Set(Tsk.Start, new DateTime(2000, 3, 15, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(3));

var assignment = project.ResourceAssignments.Add(task, project.Resources.Add("r1"));
assignment.Set(Asn.Start, new DateTime(2000, 3, 15, 8, 0, 0));
assignment.Set(Asn.Work, task.Get(Tsk.Work));
assignment.Set(Asn.Finish, new DateTime(2000, 3, 19, 17, 0, 0));

// harus menghasilkan data timephased penugasan sumber daya terlebih dahulu
assignment.TimephasedDataFromTaskDuration(project.Get(Prj.Calendar));

// pecah tugas.
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 17, 17, 0, 0), project.Get(Prj.Calendar));

// iterasi atas bagian split
Console.WriteLine("Number of split parts: " + task.SplitParts.Count);
foreach (var splitPart in task.SplitParts)
{
    Console.WriteLine("  Split Part Start: " + splitPart.Start);
    Console.WriteLine("  Split Part Finish: " + splitPart.Finish);
    Console.WriteLine();
}
```

### Lihat Juga

* class [SplitPart](../)
* namespace [Aspose.Tasks](../../splitpart/)
* assembly [Aspose.Tasks](../../../)


