---
title: "Task.Delete"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Task 方法。删除父项目任务集合中的任务及其所有分配"
type: docs
weight: 1320
url: /zh/net/aspose.tasks/task/delete/
---
## Task.Delete method

从父项目任务集合中删除任务以及其所有分配。

```csharp
public void Delete()
```

## 示例

展示如何删除任务。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Number of tasks: " + project.RootTask.Children.Count);

// 删除任务
task.Delete();

Console.WriteLine("Number of tasks: " + project.RootTask.Children.Count);
```

### 另见

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


