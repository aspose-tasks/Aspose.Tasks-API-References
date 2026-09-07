---
title: "Kelas TaskLinkCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.TaskLinkCollection. Mewakili kumpulan objek Task"
type: docs
weight: 2420
url: /id/net/aspose.tasks/tasklinkcollection/
---
## TaskLinkCollection class

Mewakili kumpulan objek [`Task`](../task/).

```csharp
public class TaskLinkCollection : IList<TaskLink>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Count](../../aspose.tasks/tasklinkcollection/count/) { get; } | Mendapatkan jumlah objek yang terdapat dalam objek `TaskLinkCollection` ini. |
| [Item](../../aspose.tasks/tasklinkcollection/item/) { get; set; } | Mengembalikan atau mengatur elemen pada indeks yang ditentukan. |
| [ParentProject](../../aspose.tasks/tasklinkcollection/parentproject/) { get; } | Mendapatkan proyek induk dari objek ResourceAssignmentCollection. proyek induk [`Project`](../project/) untuk objek ini. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_3)(TaskLink) | Ini adalah implementasi stub dari metode Add milik ICollection, yang hanya melempar NotSupportedException |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add)(Task, Task) | Mengembalikan sebuah instance Finish-Start [`TaskLink`](../tasklink/) yang telah ditambahkan ke objek TaskLinkCollection. |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_1)(Task, Task, TaskLinkType) | Mengembalikan sebuah instance [`TaskLink`](../tasklink/) yang telah ditambahkan ke objek TaskLinkCollection. |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_2)(Task, Task, TaskLinkType, Duration) | Mengembalikan sebuah instance [`TaskLink`](../tasklink/) yang telah ditambahkan ke objek TaskLinkCollection. |
| [GetEnumerator](../../aspose.tasks/tasklinkcollection/getenumerator/)() | Mengembalikan enumerator untuk koleksi ini. |
| [Remove](../../aspose.tasks/tasklinkcollection/remove/)(TaskLink) | Menghapus tautan tugas dari sebuah proyek. |
| [ToList](../../aspose.tasks/tasklinkcollection/tolist/)() | Mengonversi objek TaskLinkCollection menjadi daftar objek [`TaskLink`](../tasklink/). |

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

* class [TaskLink](../tasklink/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


