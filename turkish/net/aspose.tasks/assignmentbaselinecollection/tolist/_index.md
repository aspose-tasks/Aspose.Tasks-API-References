---
title: "AssignmentBaselineCollection.ToList"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "AssignmentBaselineCollection metodu. AssignmentBaselineCollection nesnesini AssignmentBaseline nesnelerinin bir listesine dönüştürür"
type: docs
weight: 70
url: /tr/net/aspose.tasks/assignmentbaselinecollection/tolist/
---
## AssignmentBaselineCollection.ToList method

AssignmentBaselineCollection nesnesini [`AssignmentBaseline`](../../assignmentbaseline/) nesnelerinin bir listesine dönüştürür.

```csharp
public List<AssignmentBaseline> ToList()
```

### Dönüş Değeri

[`AssignmentBaseline`](../../assignmentbaseline/) nesnelerinin listesi.

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


