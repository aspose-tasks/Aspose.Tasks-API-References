---
title: "Task.OutlineIndent"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Task 方法。在大纲中缩进任务"
type: docs
weight: 1380
url: /zh/net/aspose.tasks/task/outlineindent/
---
## Task.OutlineIndent method

在大纲中缩进任务。

```csharp
public void OutlineIndent()
```

## 示例

展示如何缩进任务。

```csharp
var project = new Project();
var task1 = project.RootTask.Children.Add("Parent");
var task2 = project.RootTask.Children.Add("Task");
Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));

// 缩进任务
task2.OutlineIndent();

Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));
```

### 另见

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


