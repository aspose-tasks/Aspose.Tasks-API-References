---
title: "AssignmentBaselineCollection.Remove"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode AssignmentBaselineCollection. Menghapus baseline dari koleksi ini"
type: docs
weight: 60
url: /id/net/aspose.tasks/assignmentbaselinecollection/remove/
---
## AssignmentBaselineCollection.Remove method

Menghapus baseline dari koleksi ini.

```csharp
public bool Remove(AssignmentBaseline item)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| item | AssignmentBaseline | Item yang akan dihapus. |

### Nilai Kembali

true jika instance [`AssignmentBaseline`](../../assignmentbaseline/) telah berhasil dihapus; jika tidak, false

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

* class [AssignmentBaseline](../../assignmentbaseline/)
* class [AssignmentBaselineCollection](../)
* namespace [Aspose.Tasks](../../assignmentbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


