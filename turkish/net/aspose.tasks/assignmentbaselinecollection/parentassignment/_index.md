---
title: "AssignmentBaselineCollection.ParentAssignment"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "AssignmentBaselineCollection özelliği. Bu koleksiyon için üst ResourceAssignment'ı alır"
type: docs
weight: 30
url: /tr/net/aspose.tasks/assignmentbaselinecollection/parentassignment/
---
## AssignmentBaselineCollection.ParentAssignment property

Bu koleksiyon için üst [`ResourceAssignment`](../../resourceassignment/) nesnesini alır.

```csharp
public ResourceAssignment ParentAssignment { get; }
```

## Örnekler

Atama temel hatlarını okumanın nasıl yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "AssignmentBaseline2007.mpp");

// Atama temel bilgilerini oku
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

// atanmış temel hatları sil
foreach (var assignment in project.ResourceAssignments)
{
    List<AssignmentBaseline> baselines = assignment.Baselines.ToList();
    foreach (var baseline in baselines)
    {
        assignment.Baselines.Remove(baseline);
    }
}
```

### Ayrıca Bakınız

* class [ResourceAssignment](../../resourceassignment/)
* class [AssignmentBaselineCollection](../)
* namespace [Aspose.Tasks](../../assignmentbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


