---
title: "ResourceAssignment.Baselines"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ResourceAssignment özelliği. AssignmentBaselineCollection nesnesini alır. Atama ile ilişkili temel değerlerin koleksiyonu"
type: docs
weight: 120
url: /tr/net/aspose.tasks/resourceassignment/baselines/
---
## ResourceAssignment.Baselines property

AssignmentBaselineCollection nesnesini alır. Atama ile ilişkili temel değerlerin koleksiyonudur.

```csharp
public AssignmentBaselineCollection Baselines { get; }
```

## Örnekler

Atamanın temel değerlerine nasıl erişileceğini gösterir.

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

### Ayrıca Bakınız

* class [AssignmentBaselineCollection](../../assignmentbaselinecollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


