---
title: "ResourceAssignment.ToString"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ResourceAssignment 方法。返回 ResourceAssignment 类实例的简短字符串表示。表示的具体细节未指定，可能会更改"
type: docs
weight: 790
url: /zh/net/aspose.tasks/resourceassignment/tostring/
---
## ResourceAssignment.ToString method

返回 [`ResourceAssignment`](../) 类实例的简短字符串表示。表示的具体细节未指定，可能会更改。

```csharp
public override string ToString()
```

### 返回值

表示分配对象的简短字符串。

## 示例

展示如何打印常见的分配信息。

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

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


