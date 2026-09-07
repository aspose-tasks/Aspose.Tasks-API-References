---
title: "SplitPart.GetHashCode"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode SplitPart. Mengembalikan nilai kode hash untuk instance dari kelas SplitPart"
type: docs
weight: 40
url: /id/net/aspose.tasks/splitpart/gethashcode/
---
## SplitPart.GetHashCode method

Mengembalikan nilai kode hash untuk instance dari kelas [`SplitPart`](../).

```csharp
public override int GetHashCode()
```

### Nilai Kembali

mengembalikan nilai kode hash untuk objek ini.

## Contoh

Menampilkan cara mendapatkan kode hash dari sebuah split part.

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

// kesetaraan bagian split diperiksa terhadap start, finish, dan index dari bagian split.
var part1 = task.SplitParts[0];
var part2 = task.SplitParts[1];

// kode hash dari sebuah split part berdasarkan start, finish, dan index dari split part.
Console.WriteLine("Split Part 1 Start {0} Finish {1} HashCode {2}", part1.Start, part1.Finish, part1.GetHashCode());
Console.WriteLine("Split Part 2 Start {0} Finish {1} HashCode {2}", part2.Start, part2.Finish, part2.GetHashCode());
```

### Lihat Juga

* class [SplitPart](../)
* namespace [Aspose.Tasks](../../splitpart/)
* assembly [Aspose.Tasks](../../../)


