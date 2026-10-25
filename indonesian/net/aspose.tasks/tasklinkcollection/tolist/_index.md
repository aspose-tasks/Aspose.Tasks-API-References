---
title: "TaskLinkCollection.ToList"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode TaskLinkCollection. Mengonversi objek TaskLinkCollection menjadi daftar objek TaskLink"
type: docs
weight: 70
url: /id/net/aspose.tasks/tasklinkcollection/tolist/
---
## TaskLinkCollection.ToList method

Mengonversi objek TaskLinkCollection menjadi daftar objek [`TaskLink`](../../tasklink/).

```csharp
public List<TaskLink> ToList()
```

### Nilai Kembali

Daftar objek [`TaskLink`](../../tasklink/).

## Contoh

Menampilkan cara bekerja dengan koleksi tautan tugas.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// dapatkan tugas
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// tautkan tugas-tugas
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// cetak tautan di antara tugas-tugas
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// sunting tautan dengan akses indeks
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// hapus semua tautan tugas
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### Lihat Juga

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)


