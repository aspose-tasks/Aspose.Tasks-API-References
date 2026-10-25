---
title: "Task.GetHashCode"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Task 方法。返回此 Task 的哈希码值。"
type: docs
weight: 1350
url: /zh/net/aspose.tasks/task/gethashcode/
---
## Task.GetHashCode method

返回此 Task 的哈希码值。

```csharp
public override int GetHashCode()
```

### 返回值

返回此对象的哈希码值。

## 示例

展示如何获取任务的哈希码。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

// 任务的哈希码基于任务的 UID 和名称
Console.WriteLine("Hash code of the task: " + task.GetHashCode());

task.Set(Tsk.Name, "Task 1");

Console.WriteLine("Hash code of the task: " + task.GetHashCode());
```

### 另见

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


