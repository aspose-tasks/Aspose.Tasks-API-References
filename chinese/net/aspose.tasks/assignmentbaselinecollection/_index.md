---
title: "类 AssignmentBaselineCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.AssignmentBaselineCollection 类。表示 AssignmentBaseline 对象的集合。"
type: docs
weight: 60
url: /zh/net/aspose.tasks/assignmentbaselinecollection/
---
## AssignmentBaselineCollection class

表示 [`AssignmentBaseline`](../assignmentbaseline/) 对象的集合。

```csharp
public class AssignmentBaselineCollection : IList<AssignmentBaseline>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/assignmentbaselinecollection/count/) { get; } | 获取此 AssignmentBaselineCollection 对象中包含的对象数量。 |
| [Item](../../aspose.tasks/assignmentbaselinecollection/item/) { get; set; } | 返回指定索引处的元素。 |
| [ParentAssignment](../../aspose.tasks/assignmentbaselinecollection/parentassignment/) { get; } | 获取此集合的父级 [`ResourceAssignment`](../resourceassignment/)。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks/assignmentbaselinecollection/add/)(AssignmentBaseline) | 这是 ICollection 的 Add 方法的存根实现，只会抛出 NotSupportedException。 |
| [GetEnumerator](../../aspose.tasks/assignmentbaselinecollection/getenumerator/)() | 返回此集合的枚举器。 |
| [Remove](../../aspose.tasks/assignmentbaselinecollection/remove/)(AssignmentBaseline) | 从此集合中移除基线。 |
| [ToList](../../aspose.tasks/assignmentbaselinecollection/tolist/)() | 将 AssignmentBaselineCollection 对象转换为 [`AssignmentBaseline`](../assignmentbaseline/) 对象的列表。 |

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

* class [AssignmentBaseline](../assignmentbaseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


