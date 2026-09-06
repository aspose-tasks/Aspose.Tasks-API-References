---
title: "AssignmentBaselineCollection.Remove"
second_title: "Aspose.Tasks for .NET API 参考"
description: "AssignmentBaselineCollection 方法。 从此集合中移除基线"
type: docs
weight: 60
url: /zh/net/aspose.tasks/assignmentbaselinecollection/remove/
---
## AssignmentBaselineCollection.Remove method

从此集合中移除基线。

```csharp
public bool Remove(AssignmentBaseline item)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | AssignmentBaseline | 要移除的项。 |

### 返回值

如果已成功删除 [`AssignmentBaseline`](../../assignmentbaseline/) 实例，则为 true；否则为 false

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


