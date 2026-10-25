---
title: "Task.OutlineOutdent"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Task method. 在大纲中提升任务"
type: docs
weight: 1390
url: /zh/net/aspose.tasks/task/outlineoutdent/
---
## Task.OutlineOutdent method

在大纲中提升任务。

```csharp
public void OutlineOutdent()
```

## 示例

展示如何向左缩进任务。

```csharp
var project = new Project();
var task1 = project.RootTask.Children.Add("Parent");
var task2 = task1.Children.Add("Task");
Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));

// 向左缩进任务
task2.OutlineOutdent();

Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));
```

### 另见

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


