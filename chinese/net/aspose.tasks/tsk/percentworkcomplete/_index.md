---
title: "Tsk.PercentWorkComplete"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk field. 以已完成工作百分比表示的任务当前状态."
type: docs
weight: 890
url: /zh/net/aspose.tasks/tsk/percentworkcomplete/
---
## Tsk.PercentWorkComplete field

任务的当前状态，以已完成的工作百分比表示。

```csharp
public static readonly Key<int, TaskKey> PercentWorkComplete;
```

## 示例

展示如何读取/写入 Tsk.PercentWorkComplete 属性.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PercentWorkComplete, 10);

Console.WriteLine("Percent Work Complete: " + task.Get(Tsk.PercentWorkComplete));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


