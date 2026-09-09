---
title: "Sınıf AssignmentBaselineCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.AssignmentBaselineCollection sınıfı. AssignmentBaseline nesnelerinin bir koleksiyonunu temsil eder."
type: docs
weight: 60
url: /tr/net/aspose.tasks/assignmentbaselinecollection/
---
## AssignmentBaselineCollection class

[`AssignmentBaseline`](../assignmentbaseline/) nesnelerinin bir koleksiyonunu temsil eder.

```csharp
public class AssignmentBaselineCollection : IList<AssignmentBaseline>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.tasks/assignmentbaselinecollection/count/) { get; } | Bu AssignmentBaselineCollection nesnesinde bulunan nesne sayısını alır. |
| [Item](../../aspose.tasks/assignmentbaselinecollection/item/) { get; set; } | Belirtilen indeksteki öğeyi döndürür. |
| [ParentAssignment](../../aspose.tasks/assignmentbaselinecollection/parentassignment/) { get; } | Bu koleksiyon için üst [`ResourceAssignment`](../resourceassignment/) nesnesini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.tasks/assignmentbaselinecollection/add/)(AssignmentBaseline) | Bu, ICollection'ın Add metodunun sadece NotSupportedException fırlatan taslak uygulamasıdır |
| [GetEnumerator](../../aspose.tasks/assignmentbaselinecollection/getenumerator/)() | Bu koleksiyon için bir enumerator döndürür. |
| [Remove](../../aspose.tasks/assignmentbaselinecollection/remove/)(AssignmentBaseline) | Bu koleksiyondan temel çizgiyi kaldırır. |
| [ToList](../../aspose.tasks/assignmentbaselinecollection/tolist/)() | AssignmentBaselineCollection nesnesini bir [`AssignmentBaseline`](../assignmentbaseline/) nesne listesine dönüştürür. |

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

* class [AssignmentBaseline](../assignmentbaseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


