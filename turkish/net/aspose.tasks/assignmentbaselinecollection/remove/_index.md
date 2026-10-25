---
title: "AssignmentBaselineCollection.Remove"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "AssignmentBaselineCollection metodu. Bu koleksiyondan temel çizgiyi kaldırır"
type: docs
weight: 60
url: /tr/net/aspose.tasks/assignmentbaselinecollection/remove/
---
## AssignmentBaselineCollection.Remove method

Bu koleksiyondan temel çizgiyi kaldırır.

```csharp
public bool Remove(AssignmentBaseline item)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| öğe | AssignmentBaseline | Kaldırılacak öğe. |

### Dönüş Değeri

Eğer [`AssignmentBaseline`](../../assignmentbaseline/) örneği başarıyla kaldırıldıysa true; aksi takdirde false

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

* class [AssignmentBaseline](../../assignmentbaseline/)
* class [AssignmentBaselineCollection](../)
* namespace [Aspose.Tasks](../../assignmentbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


