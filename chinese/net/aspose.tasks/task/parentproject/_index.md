---
title: "Task.ParentProject"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Task 属性。获取任务的父项目"
type: docs
weight: 930
url: /zh/net/aspose.tasks/task/parentproject/
---
## Task.ParentProject property

获取任务的父项目。

```csharp
public Project ParentProject { get; }
```

## 备注

调用 Project.UpdateReferences 来更新这些属性。

## 示例

展示如何使用任务的父项目。

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Parent");

// 通过使用默认项目时间单位类型为任务设置持续时间。
task.Set(Tsk.Duration, task.ParentProject.GetDuration(1));

Console.WriteLine(task.Get(Tsk.Duration));
```

### 另见

* class [Project](../../project/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


