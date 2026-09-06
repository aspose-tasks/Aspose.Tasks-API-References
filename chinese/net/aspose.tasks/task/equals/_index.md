---
title: "Task.Equals"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Task 方法。返回一个值，指示此实例是否等于指定的任务。"
type: docs
weight: 1330
url: /zh/net/aspose.tasks/task/equals/
---
## Equals(Task) {#equals}

返回一个值，指示此实例是否等于指定的任务。

```csharp
public bool Equals(Task other)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 其他 | 任务 | 指定的任务，用于与此实例比较。 |

### 返回值

如果指定的任务和此实例具有相同的唯一标识，则返回 true。

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

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

返回一个值，指示此实例是否等于指定的对象。

```csharp
public override bool Equals(object obj)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | 对象 | 指定的对象，用于与此实例比较。 |

### 返回值

如果指定的任务和此实例具有相同的唯一标识，则返回 true。

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

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


