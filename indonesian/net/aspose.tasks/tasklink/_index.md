---
title: "Kelas TaskLink"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.TaskLink. Mewakili tautan pendahulu"
type: docs
weight: 2410
url: /id/net/aspose.tasks/tasklink/
---
## TaskLink class

Mewakili tautan pendahulu.

```csharp
public sealed class TaskLink : IEquatable<TaskLink>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [CrossProjectName](../../aspose.tasks/tasklink/crossprojectname/) { get; set; } | Mendapatkan atau mengatur proyek pendahulu eksternal. |
| [IsCrossProject](../../aspose.tasks/tasklink/iscrossproject/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah pendahulu merupakan bagian dari proyek lain. |
| [LagFormat](../../aspose.tasks/tasklink/lagformat/) { get; set; } | Mendapatkan atau mengatur format untuk mengekspresikan format lag. |
| [LinkLag](../../aspose.tasks/tasklink/linklag/) { get; set; } | Mendapatkan atau mengatur lag dalam satu persepuluh menit atau persentase. |
| [LinkLagTimeSpan](../../aspose.tasks/tasklink/linklagtimespan/) { get; set; } | Mendapatkan atau mengatur durasi lag, tergantung pada LagFormat. |
| [LinkType](../../aspose.tasks/tasklink/linktype/) { get; set; } | Mendapatkan atau mengatur tipe tautan. |
| [PredTask](../../aspose.tasks/tasklink/predtask/) { get; set; } | Mendapatkan atau mengatur tugas pendahulu. |
| [SuccTask](../../aspose.tasks/tasklink/succtask/) { get; set; } | Mendapatkan atau mengatur tugas penerus. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| override [Equals](../../aspose.tasks/tasklink/equals/#equals_1)(object) | Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| [Equals](../../aspose.tasks/tasklink/equals/#equals)(TaskLink) | Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| override [GetHashCode](../../aspose.tasks/tasklink/gethashcode/)() | Mengembalikan nilai kode hash untuk instance kelas `TaskLink`. |
| override [ToString](../../aspose.tasks/tasklink/tostring/)() | Mengembalikan representasi string dari TaskLink. Detail tepat dari representasi tidak ditentukan dan dapat berubah. |

## Contoh

Menampilkan cara membaca tautan tugas proyek.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

// Tampilkan nama tugas pendahulu dan penerus
foreach (var taskLink in project.TaskLinks)
{
    Console.WriteLine("Predecessor: " + taskLink.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor: " + taskLink.SuccTask.Get(Tsk.Name));
    Console.WriteLine("Lag Format: " + taskLink.LagFormat);
    Console.WriteLine("Link Lag: " + taskLink.LinkLag);
    Console.WriteLine();
}
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


