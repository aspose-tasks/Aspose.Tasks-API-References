---
title: "AssignmentBaselineCollection.Count"
second_title: "Aspose.Tasks for .NET API 参考"
description: "AssignmentBaselineCollection 属性。获取此 AssignmentBaselineCollection 对象中包含的对象数量"
type: docs
weight: 10
url: /zh/net/aspose.tasks/assignmentbaselinecollection/count/
---
## AssignmentBaselineCollection.Count property

获取此 AssignmentBaselineCollection 对象中包含的对象数量。

```csharp
public int Count { get; }
```

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

* class [AssignmentBaselineCollection](../)
* namespace [Aspose.Tasks](../../assignmentbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


