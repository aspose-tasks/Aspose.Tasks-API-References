---
title: "ResourceAssignment.ToString"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ResourceAssignment. Mengembalikan representasi string singkat dari instance kelas ResourceAssignment. Detail tepat dari representasi tidak ditentukan dan dapat berubah."
type: docs
weight: 790
url: /id/net/aspose.tasks/resourceassignment/tostring/
---
## ResourceAssignment.ToString method

Mengembalikan representasi string singkat dari instance kelas [`ResourceAssignment`](../). Detail tepat dari representasi tidak ditentukan dan dapat berubah.

```csharp
public override string ToString()
```

### Nilai Kembali

string singkat yang mewakili objek penugasan.

## Contoh

Menampilkan cara mencetak informasi penugasan umum.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // tampilkan penugasan tugas
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### Lihat Juga

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


