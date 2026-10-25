---
title: "Kelas AssignmentBaselineCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.AssignmentBaselineCollection class. Mewakili koleksi objek AssignmentBaseline."
type: docs
weight: 60
url: /id/net/aspose.tasks/assignmentbaselinecollection/
---
## AssignmentBaselineCollection class

Mewakili koleksi objek [`AssignmentBaseline`](../assignmentbaseline/).

```csharp
public class AssignmentBaselineCollection : IList<AssignmentBaseline>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Count](../../aspose.tasks/assignmentbaselinecollection/count/) { get; } | Mendapatkan jumlah objek yang terdapat dalam objek AssignmentBaselineCollection ini. |
| [Item](../../aspose.tasks/assignmentbaselinecollection/item/) { get; set; } | Mengembalikan elemen pada indeks yang ditentukan. |
| [ParentAssignment](../../aspose.tasks/assignmentbaselinecollection/parentassignment/) { get; } | Mendapatkan induk [`ResourceAssignment`](../resourceassignment/) untuk koleksi ini. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Add](../../aspose.tasks/assignmentbaselinecollection/add/)(AssignmentBaseline) | Ini adalah implementasi stub dari metode Add milik ICollection, yang hanya melempar NotSupportedException |
| [GetEnumerator](../../aspose.tasks/assignmentbaselinecollection/getenumerator/)() | Mengembalikan enumerator untuk koleksi ini. |
| [Remove](../../aspose.tasks/assignmentbaselinecollection/remove/)(AssignmentBaseline) | Menghapus baseline dari koleksi ini. |
| [ToList](../../aspose.tasks/assignmentbaselinecollection/tolist/)() | Mengonversi objek AssignmentBaselineCollection menjadi daftar objek [`AssignmentBaseline`](../assignmentbaseline/). |

## Contoh

Menampilkan cara membaca baseline penugasan.

```csharp
var project = new Project(DataDir + "AssignmentBaseline2007.mpp");

// baca informasi baseline penugasan
foreach (var assignment in project.ResourceAssignments)
{
    var baselines = assignment.Baselines;
    Console.WriteLine("Count of assignment baselines: " + baselines.Count);
    Console.WriteLine("Parent Assignment: " + baselines.ParentAssignment);
    foreach (var baseline in baselines)
    {
        Console.WriteLine("Baseline Start: " + baseline.Start);
        Console.WriteLine("Baseline Finish: " + baseline.Finish);
    }

    Console.WriteLine();
}

Console.WriteLine("Delete all assignment baselines: ");

// hapus baseline penugasan
foreach (var assignment in project.ResourceAssignments)
{
    List<AssignmentBaseline> baselines = assignment.Baselines.ToList();
    foreach (var baseline in baselines)
    {
        assignment.Baselines.Remove(baseline);
    }
}
```

### Lihat Juga

* class [AssignmentBaseline](../assignmentbaseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


