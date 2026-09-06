---
title: "Task.Assignments"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Task 属性。获取此对象的资源分配集合。"
type: docs
weight: 120
url: /zh/net/aspose.tasks/task/assignments/
---
## Task.Assignments property

获取此对象的资源分配集合。

```csharp
public ResourceAssignmentCollection Assignments { get; }
```

## 示例

展示如何遍历任务的分配。

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // 显示任务的分配
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### 另见

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


