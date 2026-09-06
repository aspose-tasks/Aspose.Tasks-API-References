---
title: "Task.Clone"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Task 方法。创建任务的完整副本（不包括子任务）"
type: docs
weight: 1310
url: /zh/net/aspose.tasks/task/clone/
---
## Task.Clone method

创建任务的完整副本（不包括子任务）。

```csharp
public object Clone()
```

### 返回值

已创建任务的副本。

## 示例

展示如何克隆任务。

```csharp
var project = new Project();

var originalTask = project.RootTask.Children.Add("Task");
var cloneTask = (Task)originalTask.Clone();

Console.WriteLine("Are tasks equal: " + cloneTask.Equals(originalTask));
```

### 另见

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


