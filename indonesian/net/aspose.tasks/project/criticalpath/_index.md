---
title: "Project.CriticalPath"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Project. Mendapatkan koleksi yang berisi daftar tugas Critical yang membentuk Critical Path dari proyek ini. Ini adalah operasi On dimana n adalah jumlah tugas dalam proyek."
type: docs
weight: 180
url: /id/net/aspose.tasks/project/criticalpath/
---
## Project.CriticalPath property

Menampilkan koleksi yang berisi daftar tugas Critical yang membentuk Critical Path proyek ini. Ini adalah operasi O(n), di mana n adalah jumlah tugas dalam proyek.

```csharp
public TaskCollection CriticalPath { get; }
```

### Nilai Kembali

sebuah koleksi yang mewakili daftar semua tugas kritis.

## Contoh

Menampilkan cara menghitung critical path proyek.

```csharp
var project = new Project()
{
    CalculationMode = CalculationMode.Automatic
};

var subtask1 = project.RootTask.Children.Add("1");
var subtask2 = project.RootTask.Children.Add("2");
project.TaskLinks.Add(subtask1, subtask2, TaskLinkType.FinishToStart);

project.RootTask.Children.Add("3");

// Tampilkan critical path sekarang
foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id) + "  " + task.Get(Tsk.Name));
    Console.WriteLine(task.Get(Tsk.Start));
    Console.WriteLine(task.Get(Tsk.Finish) + "\n");
}
```

### Lihat Juga

* class [TaskCollection](../../taskcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


