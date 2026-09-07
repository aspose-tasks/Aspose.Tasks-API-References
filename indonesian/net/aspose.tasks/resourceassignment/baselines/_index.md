---
title: "ResourceAssignment.Baselines"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ResourceAssignment. Mendapatkan objek AssignmentBaselineCollection. Kumpulan nilai baseline yang terkait dengan penugasan"
type: docs
weight: 120
url: /id/net/aspose.tasks/resourceassignment/baselines/
---
## ResourceAssignment.Baselines property

Mendapatkan objek AssignmentBaselineCollection. Kumpulan nilai baseline yang terkait dengan sebuah penugasan.

```csharp
public AssignmentBaselineCollection Baselines { get; }
```

## Contoh

Menampilkan cara mengakses baseline penugasan.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

project.SetBaseline(BaselineType.Baseline);

foreach (var assignmentBaseline in resourceAssignment.Baselines)
{
    Console.WriteLine("Baseline Start: {0}", assignmentBaseline.Start);
    Console.WriteLine("Baseline Finish: {0}", assignmentBaseline.Finish);
}
```

### Lihat Juga

* class [AssignmentBaselineCollection](../../assignmentbaselinecollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


