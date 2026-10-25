---
title: "AssignmentBaselineCollection.Count"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti AssignmentBaselineCollection. Mendapatkan jumlah objek yang terdapat dalam objek AssignmentBaselineCollection ini"
type: docs
weight: 10
url: /id/net/aspose.tasks/assignmentbaselinecollection/count/
---
## AssignmentBaselineCollection.Count property

Mendapatkan jumlah objek yang terdapat dalam objek AssignmentBaselineCollection ini.

```csharp
public int Count { get; }
```

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

* class [AssignmentBaselineCollection](../)
* namespace [Aspose.Tasks](../../assignmentbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


