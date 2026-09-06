---
title: "ResourceAssignment.Baselines"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ResourceAssignment 属性。获取 AssignmentBaselineCollection 对象。与分配关联的基线值集合。"
type: docs
weight: 120
url: /zh/net/aspose.tasks/resourceassignment/baselines/
---
## ResourceAssignment.Baselines property

获取 AssignmentBaselineCollection 对象。该集合包含与分配关联的基线值。

```csharp
public AssignmentBaselineCollection Baselines { get; }
```

## 示例

展示如何访问分配的基线。

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

### 另见

* class [AssignmentBaselineCollection](../../assignmentbaselinecollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


