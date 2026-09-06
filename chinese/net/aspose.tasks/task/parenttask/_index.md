---
title: "Task.ParentTask"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Task 属性。获取任务的父任务"
type: docs
weight: 940
url: /zh/net/aspose.tasks/task/parenttask/
---
## Task.ParentTask property

获取任务的父任务。

```csharp
public Task ParentTask { get; }
```

## 示例

展示如何使用任务的父任务。

```csharp
var project = new Project();
var parent = project.RootTask.Children.Add("Parent");
var child1 = parent.Children.Add("Child1");
var child2 = child1.ParentTask.Children.Add("Child2");

Console.WriteLine("Is parent is equal to the root task: " + child2.ParentTask.Equals(parent));
```

### 另见

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


