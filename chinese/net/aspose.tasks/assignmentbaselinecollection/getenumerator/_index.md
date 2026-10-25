---
title: "AssignmentBaselineCollection.GetEnumerator"
second_title: "Aspose.Tasks for .NET API 参考"
description: "AssignmentBaselineCollection 方法。 返回此集合的枚举器"
type: docs
weight: 50
url: /zh/net/aspose.tasks/assignmentbaselinecollection/getenumerator/
---
## AssignmentBaselineCollection.GetEnumerator method

返回此集合的枚举器。

```csharp
public IEnumerator<AssignmentBaseline> GetEnumerator()
```

### 返回值

此集合的枚举器。

## 示例

展示如何读取分配基线。

```csharp
var project = new Project(DataDir + "AssignmentBaseline2007.mpp");

// 读取分配基线信息。
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

// 删除分配基线
foreach (var assignment in project.ResourceAssignments)
{
    List<AssignmentBaseline> baselines = assignment.Baselines.ToList();
    foreach (var baseline in baselines)
    {
        assignment.Baselines.Remove(baseline);
    }
}
```

### 另见

* class [AssignmentBaseline](../../assignmentbaseline/)
* class [AssignmentBaselineCollection](../)
* namespace [Aspose.Tasks](../../assignmentbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


