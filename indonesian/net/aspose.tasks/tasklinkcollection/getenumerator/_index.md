---
title: "TaskLinkCollection.GetEnumerator"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode TaskLinkCollection. Mengembalikan enumerator untuk koleksi ini"
type: docs
weight: 50
url: /id/net/aspose.tasks/tasklinkcollection/getenumerator/
---
## TaskLinkCollection.GetEnumerator method

Mengembalikan enumerator untuk koleksi ini.

```csharp
public IEnumerator<TaskLink> GetEnumerator()
```

### Nilai Kembali

enumerator untuk koleksi ini.

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


